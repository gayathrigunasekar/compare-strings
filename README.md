# compare-strings
compare two strings without using strcmp()
int compare(char[],char[]);
int main()
{int flag;
char a[1000],b[1000];
printf("enter first string\n");
gets(a);
printf("enter second string\n");
gets(b);
flag=compare(a,b);
if(flag==0)
printf("entered strings are equal\n");
else
printf("strings not equal\n");
return 0;}
int compare(char[a],char[b])
{ int c=0;
while(a[c]==b[c]){
if(a[c]=='\0'||b[c]=='\0')
break;
c++;
}
if(a[c]=='\0'&&b[c]=='\0')
return 0;
else
return -1;}
