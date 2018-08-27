# hello-world-
#include<stdio.h>
  int main()
  {
    
    char  str[]={"175.54.65.64"};
    puts(str);
    gets(str);
    ipv4(str);
    
  }
 char ipv4(char str[])
{   
    char arr[4];
    int i = 0;
    while (str[i] != '.')
    {
        arr[i] = str[i];
        i++;
    }
    i--;
    int ip = 0, j = 1;
    while (i >= 0)
    {
        ip = ip + (str[i] - '0') * j;
        j = j * 10;
        i--;
    }
    if (ip >=1 && ip <= 126)
{
      printf("class A")
        return 'A';
 }
    else if (ip >= 128 && ip <= 191)
{
    printf("class B");
        return 'B';
}
    else if (ip >= 192 && ip <= 223)
    {
      printf("class C");
        return 'C';
      }
    else if (ip >= 224 && ip <= 239)
{
   printf("class D");
        return 'D';
 }
   
    else
       {
          printf("class E");
          return 'E';
        }  
