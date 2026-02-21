#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int number, guess, attempts = 0;
    char choice;

    srand(time(0));   // Seed for random number

    do
    {
        number = rand() % 100 + 1;   // Random number between 1-100
        attempts = 0;

        printf("\n=== Number Guessing Game ===\n");
        printf("Guess the number between 1 and 100\n");

        do
        {
            printf("Enter your guess: ");
            scanf("%d", &guess);
            attempts++;

            if(guess > number)
                printf("Too High!\n");
            else if(guess < number)
                printf("Too Low!\n");
            else
                printf("Correct! You guessed in %d attempts.\n", attempts);

        } while(guess != number);

        printf("Do you want to play again? (y/n): ");
        scanf(" %c", &choice);

    } while(choice == 'y' || choice == 'Y');

    printf("Thank you for playing!\n");

    return 0;
}# number-guessing-game
