#include <stdio.h>
#include <string.h>

int main() {
    char cadena[100];
    int hayTriptongo = 0;
    int i;
    char c1, c2, c3;

    scanf("%s", cadena);

    for (i = 0; i < strlen(cadena) - 2; i++) {

        c1 = cadena[i];
        c2 = cadena[i + 1];
        c3 = cadena[i + 2];

        if ( c1 == 'i' || c1 == 'u' || c1 == 'y'){
            if(c2 == 'a' || c2 == 'e' || c2 == 'o'){
                if(c3 == 'i' || c3 == 'u' || c3 == 'y'){
                    hayTriptongo = 1;
                }
            }
        } 
    }
    if (hayTriptongo!=0){
        printf("La cadena contiene un triptongo\n");
    }else{
        printf("La cadena NO contiene un triptongo\n");
    }
    return 0;
}
