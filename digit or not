%{
#include <stdio.h>
%}

%%
[0-9]+	 {printf("\n%s is a digit\n",yytext);}
.	{ printf("\n%s is not a digit\n",yytext);}

%%

int yywrap(){ return 1; }

int main()
{
	printf("\nEnter a number : ");
	yylex();
	return 0;
}
