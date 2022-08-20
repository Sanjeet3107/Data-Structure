# Data-Structure
College Project
 the program of matrix multiplication in c.
 
 #include<stdio.h>
 #include<stdlib.h>
 int main(){
 int a[10],b[10][10],mul[10],r,c,i,j,k;
 
 system("cls");
 printf("enter the number of row=");
 scanf("%d",&r);
 printf("enter the number of coloumn=");
 scanf("%d",&c);
 printf("enter the first matrix element=\n");
 for(i=0;i<r;i++)
 {
 for(j=0;j<c;i++)
 {
 scanf("%d",&a[i][j]);
 }
 }
 printf("enter the sceond matrix element=\n);
 for(i=0;i<r;i++)
 {
 for(j=0;j<c;j++)
 {
 mul[i][j]=0;
 for(k=0;k<c;k++)
 {
 mul[i][j]+=a[i][k]*b[k][j];
 }
 }
 }
 //for printing result 
 for (i=0;i<r;i++)
 {
 for(j=0;j<c;j++)
 {
 printf("%d\t",mul[i][j]);
 }
 printf("\n"):
 }
 return0;
 }
