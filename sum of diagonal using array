#include <stdio.h>
#define SIZE 3
int main()
{
    printf("sum of the diagonal using array\n");
    printf("vijayalakshmi G, 192321080\n");
    int matrix[SIZE][SIZE];
    int i, j, sum = 0;

    printf("Enter elements of the %dx%d matrix:\n", SIZE, SIZE);
    for (i = 0; i < SIZE; ++i)
    {
        for (j = 0; j < SIZE; ++j)
        {
            printf("Enter element [%d][%d]: ", i + 1, j + 1);
            scanf("%d", &matrix[i][j]);
        }
    }

    printf("Matrix elements are:\n");
    for (i = 0; i < SIZE; ++i)
    {
        for (j = 0; j < SIZE; ++j)
        {
            printf("%d\t", matrix[i][j]);
            if (i == j)
            {
                sum += matrix[i][j];
            }
        }
        printf("\n");
    }

    printf("Sum of diagonal elements: %d\n", sum);

    return 0;
}

