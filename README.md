# My-Programs

// Here each alphabet in the entered string represents a candy, so to calculate how many different types of candies we have this is the code. 
#include<stdio.h>
#include<string.h>
int main(){
  char s1[100];int count=0;
  scanf("%[^\n]s",s1);
  strupr(s1);
  for (int i = 65; i <=90; i++)
  {
    int flag=0;
    for (int j = 0; s1[j]; j++)
    {
        if (s1[j]==i)
        {
          flag=1;
        }
        
    }
    if (flag)
    {
      count++;
    }
    
    
  }
  printf("%d",count);
  

return 0;
}
