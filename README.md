#include<studio.h>
#include<conio.h>
main()
{
 int m,n,i,j,first [10][10],second[10][10],res[10][10];
 clrscr();
 printf("enter the order of first matrix\n");
 scanf("%d%d",&m,&n);
 printf("enter the order of second matrix\n");
 scanf("%d%d",&p,&q);
 if (n!=p)
 {
  printf("multiplication is not possible");
 }
 else
 {
  printf("enter %d values into first matrix \n",(m*n));
  for(i=0;i<m;i++)
   {
    for (j=0;j<n;j++)
    {
     scanf(”%d",&first [i][j]);
    }
   printf(”enter %d values in to second matrix \n",(p*q));
   for(i=0;i<p;i++)
    {
     for (j=0;j<q;j++)
     {
      scanf("%d",& second [i][j]);
     }
    }
    for(i=0;i<m;i++)
     {
      for(j=0;j<q;j++)
      {
       res[i][j]=0;
       for(k=0;k<n;k++)
       {
        red[i][j]=red[i][j]+first[i][k]*second[k][j]
        }
       }
    }
    printf("the multiplication is \n");
    for(i=0;i<m;i++)
    {
     for(j=0;j<q;j++)
     {
      printf("%d\t",red[i][j]);
     }
     printf("\n");
    }
   }
}
