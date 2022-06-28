#include<stdio.h>
unsigned long amount=10000,withdraw,deposit;
int choice,pin,k;
char transaction ='y';

void main()
{
    while (pin!=5090)
    {
        printf("Enter your secret pin number : ");
        scanf("%d",&pin);
        if(pin!=5090)
        printf("PLEASE ENTER VALID PASSWARD\n");  
    }
    do
    {
        printf("---------  WELCOME TO ATM SERVICES  ----------\n\n\n");
        printf("1.Check your account balance : \n");
        printf("2.withdraw ammount \n");
        printf("3.deposit ammount \n");
        printf("4.Quit\n");
        printf("**********************************************\n\n");
        printf("Please enter your choice : ");
        scanf("%d",&choice);
        switch(choice)
        {
            case 1:
            printf("\n Your bank balance in rupees : %lu",amount);
            break;
            case 2:
            printf("\n ENTER AMOUNT TO WITHDRAW : ");
            scanf("%lu",&withdraw);
            if(withdraw %100 !=0){
                printf("PLEASE ENTER AMOUNT IN MULTIPLES OF HUNDRED");
            }
            else if(withdraw > (amount - 500)){
                printf("INSUFFICIENT BALANCE");
            }
            else{
                amount=amount-withdraw;
                printf("\n\nPLEASE COLLECT YOUR CASH");
                printf("\ncurrent balance in your account : %lu",amount);
            }
            break;
            case 3:
            printf("Please enter amount to deposit : ");
            scanf("%lu",&deposit);
            amount=amount+deposit;
            printf("YOUR CURRENT BNK BALANCE : %lu",amount);
            break;
            case 4:
            printf("\n THANK YOU FOR USING OUR ATM");
            break;
            default:
            printf("\n INVALID CHOICE");
        }
        printf("\n----- DO YOU WISH TO HAVE ANY OTHER TRANSCATION?(y/n) \n");
        scanf("%s",&transaction);
        if(transaction == 'n'|| transaction == 'N')
        k=1;
    }
    while (!k);
    printf("\n\n THANK YOU FOR USING OUR SERVICES  ");
}
