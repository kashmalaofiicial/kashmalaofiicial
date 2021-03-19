- 👋 Hi, I’m @kashmalaofiicial
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
kashmalaofiicial/kashmalaofiicial is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
#include <stdio.h>
#include <stdlib.h>

int main()
{
    float convertfrom;
    float convertto;
    float value;
    printf("\n \t\t\t\t ====================\n");
    printf(" \t\t\t\t{ The Area Converter }");
    printf("\n \t\t\t\t ====================\n");

    printf("\n Enter The Value You Want To Convert = ");
    scanf("%f",&value);

    printf("\n \t\t\t \t ********************\n");
    printf(" \t\t\t\t{ Measurement Options }");
    printf("\n \t\t\t \t ********************\n");
    printf(" \n  Press 1 For Square Foot .\n");
    printf(" \n  Press 2 For Meter .\n");
    printf(" \n  Press 3 For Inches .\n");

    printf("\n  Select Any Option You Want To Convert From = ");
    scanf("%f",&convertfrom);

    printf("\n \t\t\t \t ********************\n");
    printf(" \n  Press 1 For Square Foot .\n");
    printf(" \n  Press 2 For Meter .\n");
    printf(" \n  Press 3 For Inches .\n");

    printf("\n  Select Any Option You Want To Convert To = ");
    scanf("%f",&convertto);

//SQUARE FOOT START
    if(convertfrom==1 && convertto==1){
         printf("\n \t\t\t \t ********************");
        printf("\n \n \t\t\t{ %.1f Square Foot = %.1f Square Foot }\n \n ",value,value);
    }
    if(convertfrom==1 && convertto==2){
        printf("\n \t\t\t \t ********************");
        float result=value/10.764/2;
        printf("\n \n \t\t\t{ %.1f Square Foot = %.1f Meter }\n \n ",value,result);
    }
    if(convertfrom==1 && convertto==3){
        printf("\n \t\t\t \t ********************");
        float result=value*144/2;
        printf("\n \n \t\t\t{ %.1f Square Foot = %.1f Inches }\n \n ",value,result);
    }
//SQUARE FOOT ENDS

//METER START
    if(convertfrom==2 && convertto==1){
        printf("\n \t\t\t \t ********************");
        float result=value*2*10.764;
        printf("\n \n \t\t\t{ %.1f Meters = %.1f Square Foot }\n \n ",value,result);
    }
    if(convertfrom==2 && convertto==2){
        printf("\n \t\t\t \t ********************");
        printf("\n \n \t\t\t{ %.1f Meters = %.1f Meters}\n \n ",value,value);
    }
    if(convertfrom==2 && convertto==3){
        printf("\n \t\t\t \t ********************");
        float result=value*39.37;
        printf("\n \n \t\t\t{ %.1f Meters = %.1f Inches }\n \n ",value,result);
    }
//METER ENDS

//INCH START
  if(convertfrom==3 && convertto==1){
        printf("\n \t\t\t \t ********************");
        float result=value*2/144;
        printf("\n \n \t\t\t{ %.1f Inches = %.1f Square Foot }\n \n ",value,result);
    }
  if(convertfrom==3 && convertto==2){
        printf("\n \t\t\t \t ********************");
        float result=value/39.37;
        printf("\n \n \t\t\t{ %.1f Inches = %.1f Meters }\n \n ",value,result);
    }
    if(convertfrom==3 && convertto==3){
        printf("\n \t\t\t \t ********************");
        printf("\n \n \t\t\t{ %.1f Inches = %.1f Inches }\n \n ",value,value);
    }
//INCH ENDS

}
