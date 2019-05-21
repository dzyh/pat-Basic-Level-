#include<stdio.h>
#include<stdlib.h>

void del(int i);


int main()
{
	int n;
	int i;
	int h;
	scanf("%d", &n);
	int *p = (int *)malloc(n * sizeof(int));
	for (i = 0; i < n - 1; i++) {
		scanf("%d ", &p[i]);
	}
	scanf("%d", &p[n]);
	for (i = 0; i < 0; i++) {
		del(i);
	}
	n = sizeof(*p);
	printf("%d", n);
	for (i = 0; i < n; i++) {
		 
	}

}