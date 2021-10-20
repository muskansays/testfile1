# testfile1
Write an algo to sort an array using C
STEP 1: START
STEP 2: INITIALIZE arr1[] ={14, 29, 18, 6, 1 }
STEP 3: SET temp = 0
STEP 4: length= sizeof(arr1)/sizeof(arr1[0])
STEP 5: PRINT "Elements of Array are :"
STEP 6: SET j=0. REPEAT STEP 7 and STEP 8 UNTIL j<length
STEP 7: PRINT arr1[j]
STEP 8: j=j+1.
STEP 9: SET k=0. REPEAT STEP 10 to STEP UNTIL j<n
STEP 10: SET k=j+1. REPEAT STEP 11 UNTIL j<length
STEP 11: if(arr[j]>arr[k]) then
              temp = arr[j]
              arr[j]=arr[k]
              arr[k]=temp
STEP 12: k=k+1.
STEP 13: j=j+1.
STEP 14: PRINT new line
STEP 15: PRINT "Elements of array are sorted in ascending order"
STEP 16: SET j=0. REPEAT STEP 17 and STEP 18 UNTIL j<length
STEP 17: PRINT arr1[j]
STEP 18: j=j+1.
STEP 19: RETURN 0.
STEP 20: END.
                                                            //code
#include <stdio.h>
void main (){
   int num[];
   int i, j, a, n;
   printf("enter number of elements in an array\n");
   scanf("%d", &n);
   printf("Enter the elements\n");
   for (i = 0; i < n; ++i)
      scanf("%d", &num[i]);
   for (i = 0; i < n; ++i){
      for (j = i + 1; j < n; ++j){
         if (num[i] > num[j]){
            a = num[i];
            num[i] = num[j];
            num[j] = a;
         }
      }
   }
   printf("The numbers in ascending order is:\n");
   for (i = 0; i < n; ++i){
      printf("%d\n", num[i]);
   }
}
