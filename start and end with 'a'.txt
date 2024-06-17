#include<stdio.h>
#include<string.h>
int main()
{
	char string[100];
	int i,a,len;

	printf("enter the string:");
	scanf("%s",string);
	len=strlen(string);
	if(string[0]=='a'&&string[len-1]=='a')
	{
		for(i=0;i<len;i++)
		{
			if(string[i]=='0'||string[i]=='1')
			{
				printf("invalid\n");
				return 0;
			}
		}
		printf("accepted");
	}
	else
	{
		printf("not accepted");
	}
	return 0;
}
