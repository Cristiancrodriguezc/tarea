
#include <stdio.h>

/* DECLARACION DE VARIABLES */

/* ALUMNO 1 */
    char nombre1[80];
    float n11, n12, n13, media1;

/* ALUMNO 2 */
    char nombre2[80];
    float n21, n22, n23, media2;

/* ALUMNO 3 */
    char nombre3[80];
    float n31, n32, n33, media3;

/* ALUMNO 4 */
    char nombre4[80];
    float n41, n42, n43, media4;

/* ALUMNO 5 */
    char nombre5[80];
    float n51, n52, n53, media5;


int main(void)
{
    /* PETICION DE INFORMACION */
    
    /* ALUMNO 1 */
    
    printf("Escriba el nombre del alumno 1: ");
    gets(nombre1);
    printf("\nEscriba la primera calificación del alumno 1: ");
    scanf("%f", &n11);
    printf("Escriba la segunda calificación del alumno 1: ");
    scanf("%f", &n12);
    printf("Escriba la tercera calificación del alumno 1: ");
    scanf("%f%*c",&n13);
    /* Obsérvese que mediante %*c descartamos el \n */
    
    /* ALUMNO 2 */
    
    printf("\nEscriba el nombre del alumno 2: ");
    gets(nombre2);
    printf("\nEscriba la primera calificación del alumno 2: ");
    scanf("%f", &n21);
    printf("Escriba la segunda calificación del alumno 2: ");
    scanf("%f", &n22);
    printf("Escriba la tercera calificación del alumno 2: ");
    scanf("%f%*c",&n23);
    
    
    /* ALUMNO 3 */
    
    printf("\nEscriba el nombre del alumno 3: ");
    gets(nombre3);
    printf("\nEscriba la primera calificación del alumno 3: ");
    scanf("%f", &n31);
    printf("Escriba la segunda calificación del alumno 3: ");
    scanf("%f", &n32);
    printf("Escriba la tercera calificación del alumno 3: ");
    scanf("%f%*c",&n33);
    
    
    /* ALUMNO 4 */
    
    printf("\nEscriba el nombre del alumno 4: ");
    gets(nombre4);
    printf("\nEscriba la primera calificación del alumno 4: ");
    scanf("%f", &n41);
    printf("Escriba la segunda calificación del alumno 4: ");
    scanf("%f", &n42);
    printf("Escriba la tercera calificación del alumno 4: ");
    scanf("%f%*c",&n43);
    
    
    /* ALUMNO 5 */
    
    printf("\nEscriba el nombre del alumno 5: ");
    gets(nombre5);
    printf("\nEscriba la primera calificación del alumno 5: ");
    scanf("%f", &n51);
    printf("Escriba la segunda calificación del alumno 5: ");
    scanf("%f", &n52);
    printf("Escriba la tercera calificación del alumno 5: ");
    scanf("%f%*c",&n53);
    
    /* FASE DE CALCULOS */
    
    media1 = (n11 + n12 + n13) / 3.0;
    media2 = (n21 + n22 + n23) / 3.0;
    media3 = (n31 + n32 + n33) / 3.0;
    media5 = (n41 + n42 + n43) / 3.0;
    media5 = (n51 + n52 + n53) / 3.0;
    
    /* FASE DE IMPRESION DE RESULTADOS */
    
    printf("\n\nEl alumno 1, D. %18s, tiene la calificación %3.2f.\n",
             nombre1, media1);
    printf("El alumno 2, D. %18s, tiene la calificación %3.2f.\n",
             nombre2, media2);
    printf("El alumno 3, D. %18s, tiene la calificación %3.2f.\n",
             nombre3, media3);
    printf("El alumno 4, D. %18s, tiene la calificación %3.2f.\n",
             nombre4, media4);
    printf("El alumno 5, D. %18s, tiene la calificación %3.2f.\n",
             nombre5, media5);
    
    /* Obsérvese el uso de %18s y de %3.2f. ¿Qué significan? */
    /* Fase de terminación */
    printf("\n\nTerminación normal del programa.\n\n");
    return 0;
}
