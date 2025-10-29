# PGCD-N
Le PGCD (Plus Grand Commun Diviseur) de deux nombres est le plus grand nombre entier qui divise les deux nombres sans reste. Voici un programme qui codé avec C qui nous permet de calculer le PGCD♡





#include <stdio.h>
int main() {
    int N, L, X;
    //  Lecture des deux nombres
    printf("Entrez deux nombres entiers : ");
    
    scanf("%d %d", &N, &L);
    
    //  Tant que L n'est pas nul
    while (L != 0) {
        X = L;      // Gardons la valeur de L
        L = N % L;     // L devient le reste de N divisé par L
        N = X;      // N prend l’ancienne valeur de L
    }

    //   Affichage du résultat

    printf("Le PGCD est : %d\n", N);

    return 0;
}
