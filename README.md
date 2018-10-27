# C ismétlés

## Struktúrák
Példa:
````C
struct Books {
   char  title[50];
   char  author[50];
   char  subject[100];
   int   book_id;
} book;
````
Általános: 
````C
struct [structure tag] {

   member definition;
   member definition;
   ...
   member definition;
} [one or more structure variables];  
````
forrás: https://www.tutorialspoint.com/cprogramming/c_structures.htm


## Idő
> Az idő lekérésére számos mód létezik, alább csak egyet választok és az a `TIME()` függvény aminek előfeltétele a `<time.h>` és a `<stdio.h>`.
példa:
````C
#include <stdio.h>
#include <time.h>
int main ()
{
    time_t seconds;
    seconds = time (NULL);

    printf ("Number of hours since 1970 Jan 1st " \
            "is %ld \n", seconds/3600);
    return 0;
}
````
kimenet: `Number of hours since 1970 Jan 1st is 374528`

forrás: https://fresh2refresh.com/c-programming/c-time-related-functions/

## Függvények
általános: 
````C
return_type function_name( parameter list ) {
   body of the function
}
````
forrás: https://www.tutorialspoint.com/cprogramming/c_functions.htm

## String kezelés
````C
#include<stdio.h>
#include<string.h>

#define MAX_STRING_LEN 80

int main() {
  
  /* strings are array of characters 
   * terminated by the NULL character
   * which is different from '0' */
  
  char S[MAX_STRING_LEN];
    /******/
    ````
forrás: https://cs.nyu.edu/courses/spring05/V22.0201-001/c_tutorial/classes/String.html
