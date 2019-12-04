# Projekt-programowanie
Praca na zajecia z programowania

tutaj bedziemy pracowac nad projektem z programowania
Bartosz Lewandowski 04.12.19

#include <stdio.h>
#include <stdlib.h>



void wypisz(char plansza[6][6])
{
    printf("[%c][%c][%c][%c][%c][%c]\n",plansza[0][0],plansza[0][1],plansza[0][2],plansza[0][3],plansza[0][4],plansza[0][5]);
    printf("[%c][%c][%c][%c][%c][%c]\n",plansza[1][0],plansza[1][1],plansza[1][2],plansza[1][3],plansza[1][4],plansza[1][5]);
    printf("[%c][%c][%c][%c][%c][%c]\n",plansza[2][0],plansza[2][1],plansza[2][2],plansza[2][3],plansza[2][4],plansza[2][5]);
}

int pelna(char plansza[6][6])
{
    int i,j;
        for(i=0;i<6;i++)
            if(plansza[i][j] == ' ')
            return 0;
    return 1;        
}
void ruch_gracza(char plansza[6][6])
{
    unsigned int i=6, j;
    wypisz(plansza);
    
}

char sprawdz(char plansza[6][6])
{
    int i;
    for(i=0; i<6;i++)
    {
        if((plansza[i][0]!=' ')
        && (plansza[i][0]==plansza[i][1])
        && (plansza[i][0]==plansza[i][2])
        && (plansza[i][0]==plansza[i][3])
        && (plansza[i][0]==plansza[i][4])
        && (plansza[i][0]==plansza[i][5]))
        return plansza[i][0];
        if((plansza[0][i]!=' ')
        && (plansza[i][0]==plansza[1][i])
        && (plansza[i][0]==plansza[2][i])
        && (plansza[i][0]==plansza[3][i])
        && (plansza[i][0]==plansza[4][i])
        && (plansza[i][0]==plansza[5][i]))
        return plansza[0][i];
    }
        if((plansza[0][0]!=' ')
        && (plansza[0][0]==plansza[1][1])
        && (plansza[0][0]==plansza[2][2])
        && (plansza[0][0]==plansza[3][3])
        && (plansza[0][0]==plansza[4][4])
        && (plansza[0][0]==plansza[5][5]))
        return plansza[0][0];
    /* dopisac wiecej mozliwych kombinacji, refaktoryzacja */
    if (pelna(plansza)==1)
        return 1;
    return 0;
}
/* dopisac program ktory wczytuje jakieś ułożenie z plików*/ 
/*skorzystac z algorytmu alfa beta*/

int main(int argc, char *argv[])
{
    int ruch = 1;
    char wynik = 0;
    char plansza [6][6];


}


