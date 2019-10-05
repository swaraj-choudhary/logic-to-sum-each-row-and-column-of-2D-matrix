# logic-to-sum-each-row-and-column-of-2D-matrix
/*logic to sum each row and column of 2D matrix and logic would be clear to everyone.*/

#include<stdio.h>
#define size 3
int main()
{
    int array[size][size],sum_row,sum_col,i,j;
    printf("enter the elements of the array\n");
    for(i=0;i<size;i++)
    {
        for(j=0;j<size;j++)
        {
            scanf("%d\n",&array[i][j]);
        }
    }
    
    printf("Actually the sum of the every row and column present in the matrix\n");
    for(i=0;i<size;i++)
    {
        for(j=0;j<size;j++)
        {
            sum_row=sum_row+array[i][j];
            if(j==size-1)
            {
            printf("the sum of the corresponding rows: %d\n",sum_row);
            }
        }
        printf("\n");
        sum_row=0;
    }
    printf("Actually now calculating the sum of very columns:\n");
    for(i=0;i<size;i++)
    {
        for(j=0;j<size;j++)
        {
            sum_col=sum_col+array[j][i];
            if(j==size-1)
            {
            printf("the sum of the corresponding columns  in sequence: %d\n",sum_col);
            }
        }
        printf("\n");
        sum_col=0;
    }
    return 0;
}

