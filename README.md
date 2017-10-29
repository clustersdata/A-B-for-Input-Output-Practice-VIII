# A-B-for-Input-Output-Practice-VIII-

A+B for Input-Output Practice (VIII)

Problem Description

Your task is to calculate the sum of some integers. 


Input

Input contains an integer N in the first line, and then N lines follow. Each line starts with a integer M, and then M integers follow in the same line. 

 
Output

For each group of input integers you should output their sum in one line, and you must note that there is a blank line between outputs. 


Sample Input

3

4 1 2 3 4

5 1 2 3 4 5

3 1 2 3 


Sample Output

10

15

6 



解答：

int main()

{

    int a,b,i,j,l[1000],k;
    
    scanf("%d",&i);
    
    getchar();
    
    for(j=1;j<=i;j++)
    
        l[j]=0;
        
    for(j=1;j<=i;j++)
    
    {
    
        scanf("%d",&a);
        
        getchar();
        
        for(k=1;k<=a;k++)
        
        {
        
            scanf("%d",&b);
            
            getchar();
            
            l[j]+=b;
            
        }
        

    }
    
    for(j=1;j<=i-1;j++)
    
        printf("%d\n\n",l[j]);
        
    printf("%d\n",l[i]);
    

} 
