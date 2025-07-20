# find-largest-no.-in-given-array-elements.c
// C program to find largest no. in given array elements
#include <stdio.h>

int main() {
    int s,l,i;

    printf("Enter the size of the array: ");
    scanf("%d", &s);

    int a[s]; 
    printf("Enter elements:\n");
    
    for (int i=0;i<s;i++)
        scanf("%d", &a[i]);
        
        l=a[0];
    for (int i = 1; i < s; i++)
        if(l<a[i])
        l=a[i];
    printf("largest no.=%d",l);
    return 0;
}
