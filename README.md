# Array_Deletion
Deletion of a element from a given position
//1905622 - NITISH KUMAR SONTHALIA
//DELETION
#include <stdio.h>

int main()
{
    int i,n;  
 
    printf("Enter size of array: ");
    scanf("%d",&n);
    int a[100];
 
     printf("Enter %d elements in the array : ", n);
    for(i=0;i<n;i++)
    {
        scanf("%d", &a[i]);
    }
 
    printf("\nElements in array are: ");
    for(i=0;i<n;i++)
 
    {
        printf("%d  ", a[i]);
    }
    
    int s;
    printf("Enter position to delete: ");
    scanf("%d",&s);
        for ( i = s; i < n; i++)
        {
            a[i]=a[i+1];
        }
        n=n-1; 
     for(i=0;i<n;i++)
    {
        printf("%d ", a[i]);
    }

    return 0;
}
