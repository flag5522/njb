//# njb
//Academic projects for 5th Sem, B.Tech , CSE
#include <stdio.h>
int main()
{
    char ip;
    float kmtomiles = 0.621371;
    float miletokm = 1.60934;
    float poundtokg = 0.453592;
    float kgtopound = 2.20462;
    float metertofeet = 3.28084;
    float feettomet = 0.3048;
    float first, second;

    printf(" press q to quit\n press 1 for km to miles\n press 2 for miles to km\n press 3 for pound to kg\n press 4 for kg to pound\n press 5 for meter to feet\n press 6 for feet to meter\n :");
    scanf("%c", &ip);

    switch (ip)
    {
    case 'q':
        printf("you have quit the program");
        break;

    case '1':
        printf("ehter value :");
        scanf("%f", &first);
        second = first * kmtomiles;
        printf("%f km = %f miles", first, second);
        break;

    case '6':
        printf("ehter value :");
        scanf("%f", &first);
        second = first * feettomet;
        printf("%f feet = %f meters", first, second);
        break;

    case '2':
        printf("ehter value :");
        scanf("%f", &first);
        second = first * miletokm;
        printf("%f miles = %f km", first, second);
        break;

    case '3':
        printf("ehter value :");
        scanf("%f", &first);
        second = first * poundtokg;
        printf("%f pounds = %f kg", first, second);
        break;

    case '4':
        printf("ehter value :");
        scanf("%f", &first);
        second = first * kgtopound;
        printf("%f kg = %f pound", first, second);
        break;

    case '5':
        printf("ehter value :");
        scanf("%f", &first);
        second = first * metertofeet;
        printf("%f meters = %f feet", first, second);
        break;
    }

    return 0;
}
