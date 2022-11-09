# #include<stdio.h>
#include<conio.h>

int main()
{
	 long int number, rem, reverse=0;
	 clrscr();
	 printf("Enter number: ");
	 scanf("%ld", &number);
	
	 /* Reversing number */
	 while(number!=0)
	 {
		  rem = number%10;
		  reverse = reverse * 10 + rem;
		  number = number/10;
	 }
	 while(reverse != 0)
	 {
		  rem = reverse%10;
		  
		  switch(rem)
		  {
			   case 0: printf("Zero "); break;
			   case 1: printf("One "); break;
			   case 2: printf("Two "); break;
			   case 3: printf("Three "); break;
			   case 4: printf("Four "); break;
			   case 5: printf("Five "); break;
			   case 6: printf("Six "); break;
			   case 7: printf("Seven "); break;
			   case 8: printf("Eight "); break;
			   case 9: printf("Nine "); break;
		  }
		  
		  reverse = reverse/10;
	 }
	 getch();
	 return(0);
}
