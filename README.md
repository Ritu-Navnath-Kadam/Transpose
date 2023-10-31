# Transpose
#include<stdio.h>
void main()
{
int r,c,sum=0;
printf("Enter a number of rows : ");
scanf("%d",&r);
printf("Enter a number of columns : ");
scanf("%d",&c);

int arr[r][c];

for(int i=0;i<r;i++)
{
    for(int j=0;j<c;j++)
        {    
            scanf("%d",&arr[i][j]);
        }
}

printf("\n");
{printf("Given matrix");}
printf("\n");
for(int i=0;i<r;i++)
{
    for(int j=0;j<c;j++)
        {    
            printf("%d ",arr[i][j]);
        
        }
        printf("\n");
        
}

printf("\n");
for(int i=0;i<r;i++)
{
    for(int j=0;j<c;j++)
        {
        int temp=arr[i][j];
        arr[i][j]=arr[j][i];
        arr[j][i]=temp;
        
        }
      printf("\n");

}

{printf("The Transpose of given matrix\n");}
for(int i=0;i<r;i++)
{
    for(int j=0;j<c;j++)
        {
        printf("%d ",arr[j][i]);
}
printf("\n");
}
printf("\n");
}
