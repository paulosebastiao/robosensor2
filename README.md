
	#include <stdio.h>
	#include <stdlib.h>

	int main()
	{
	 char sd, sm, se, md, me;
	 loop:
	 scanf("%c %c %c", &se, &sm, &sd);
	 if((se == 0) && (sm == 0) && (sd == 0)){
	    me = 1;
	    md = 1;
	 }
	 else if (((se == 1) && (sm == 1) && (sd == 0)) || ((se == 1) && (sm == 0) && (sd == 0))) {
	    me = 1;
	    md = 0;
	 }
	 else{
	    me = 0;
	    md = 1;
	 }
	 printf("me = %d, md = %d", me, md);
	goto loop;
	    return 0;
	}
