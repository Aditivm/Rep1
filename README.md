# Rep1
#include<stdio.h>
//Loop for two terms in single iteration

main()
{
	int n, i, first_term, second_term;
	
	scanf("%d",&n);
	
	first_term = 0;
	second_term = 1;
	i=2;
	
	while(i<n)
	{
		first_term = first_term + second_term;
		second_term = first_term + second_term ; 
		
		i = i+2;
	}
	
	if(n %2 == 1)
	    printf("%dth term of fibonacci series is %d", n, first_term);
	else
	    printf("%dth term of fibonacci series is %d", n, second_term);
}
