#include<stdio.h>
int main()
{
	int n,i;
	int x=y=m=0;
	int h=100;

	scanf("%d",&n);
	struct student{
		char name[10];
		char num[10];
		int grade;
	}list[n];


	
	for(i=0,i<n,i++){
	list[i].name=gets();
	list[i].num=gets();
	scanf("%d",&list[i].grade);
	}
	for(i=0,i<n,i++){
		if(list[i].grade>m){m=list[i].grade;x=i;}
		if(list[i].grade<h){h=list[i].grade;y=i;}
	}
	printf("%s ",list[x].name);
	printf("%s\n",list[x].num);
	printf("%s ",list[y].name);
	printf("%s\n",list[y].num);
	return 0;
}