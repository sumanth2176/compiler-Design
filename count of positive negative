%{
#include <stdio.h>
int positive_no = 0, negative_no = 0;
%}

%%
[-][0-9]+	{negative_no++; printf("negative number = %s\n",yytext);}
[0-9]+	{positive_no++; printf("positive number = %s\n",yytext);}

%%

int yywrap() {
    return 1;
}

int main()
{
    printf("\nEnter a number: ");
    yylex();
    printf("\nNumber of positive numbers = %d\n", positive_no);
    printf("\nNumber of negative numbers = %d\n", negative_no);
    printf("\n");
    return 0;
}
