#include<stdio.h>
#include<string.h>
int main()
{
	char string[100];
	printf("enter the string ");
	scanf("%s",string);
	if(string[0]=='0'&&string[strlen(string)-1]=='1')
	{
		int i;
		for(i=0;i<strlen(string);i++)
		{
			if(string[i]<'0'||string[i]>'1')
			{
				printf("invalid input\n");
				return 0;
			}
		}
		printf("valid\n");
	}
	else
	{
		printf("invalid\n");
	}
	return 0;
}
