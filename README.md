# Guessing-game.c
Guessing gami in C
#include <stdio.h>
#include<stdlib.h>
int main (){
int secretNumber=7;
int guess;
int guessCount=0;
int guessLimit=3;
int outofguesses=0;
while(guess!=secretNumber&&outofguesses == 0){
    if(guessCount<guessLimit){
    printf("PLease enter a number: ");
    scanf("%d",&guess);
    guessCount++;
    }else{
    outofguesses=1;    
    }
}
if(outofguesses==1){
printf("Out of guesses \n") ;   
}else{
printf("You won");
   
}
    return 0;
}
