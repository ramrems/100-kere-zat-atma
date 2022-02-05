#include <stdio.h>
#include <stdlib.h>
#include<time.h>
int main(){
    int i,j,x,y,c=0;
    int a[2];
    srand(time(NULL));
    printf("kac kez tekrarlandigini ogrenmek istediginiz zar ciftini giriniz");
    scanf("%d",&x);
    scanf("%d",&y);
    printf("x:%d y:%d\n",x,y);
    for(j=0;j<100; j++){
    for(i=0; i<2; i++){
    a[i]=rand()% 6+1;
    printf("%d ",a[i]);}
    if (a[0]==x && a[1]==y){
      c++;}
    printf("\n");}

   printf("girdiginiz cıft %d kere tekrarlanmis",c);
