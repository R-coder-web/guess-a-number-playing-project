# guess-a-number-playing-project
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
int main(){
    int guess,random;
    int numberofguesses=0;
    srand(time(NULL));
    printf("welcome to the world of guessing number\n: ");
    random=rand()%100+1;//generating between 0 to 100
    do{
        printf("\n please enter your guess number between 1 to 100:  ");
        scanf("%d",&guess);
        numberofguesses++;
        if(guess>random){
            printf("guess a smaller number\n: ");}
            else if(guess<random){
                printf("guess a larger number\n: ");
            }
        
else{
    printf("congratulations!!!you have successfully guessed the number in %d attempts",numberofguesses);
}        
    }        
        
        while(guess!=random);
    printf("\n bye bye ,thanks for playing.");
    printf("\n Developed by:Mhr Rifat");
    return 0;
}
    
    
    
    
    
    
