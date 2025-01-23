Pyramid number pattern
In this section, we learn how to print pyramid number pattern in the java. 

here  we create half pyramid, inverted half pyramid and the triangle pyramid using a number in java.

this pattern example are useful also in interview question in java, so see every step carefully of each pattern.

To create a simple number pattern using , you have to use two loop. Due to this, nested for loop define rows to create with the columns of the number.

The first for loop define the number of rows for the pattern. The second Loop prints each row with the number.

number pattern
1. Write the Program to print the following pattern
Enter the row 5

1
1 2
1 2 3 
1 2 3 4
1 2 3 4 5
Working
Step 1-  first we need to initialize two variable for loop.

Step 2- The first loop work for the row. so loop work from 1 to row;

Step 3- The second loop work for the number in a row. so this loop work from 1 to i.

Step 4. Inside the second loop, print the j.

Step 5- Outside the second loop and inside the first loop, give new line.

 Step 6- Stop.

C	JAVA	Python	C++
#include<iostream>
using namespace std;
  
int main()  
{
    int i,  j, n;
    cin>>n;
    for(i=1; i<=n; i++)
    {
        for(j=1; j<=i; j++)
        cout<<j;
        
        
        cout<<endl;
    }    
    return 0;
}  
2. Write a program to print the following pattern
Enter number  5

1 2 3 4 5
1 2 3 4
1 2 3
1 2 
1
C	JAVA	Python	C++
#include<iostream>
using namespace std;

int main()  
{
    int i,  j, n;
    cin>>n;
    
    for(i=n; i>=1; i--)
    {
        for(j=1; j<=i; j++)
        {
            cout<<j;
        }
        cout<<endl;
    }   
    return 0;
}
3. Write a program to print the following pattern
Enter the row 5

             1
           2 3 2
         3 4 5 4 3
       4 5 6 7 6 5 4
     5 6 7 8 9 8 7 6 5
C	JAVA	Python	C++
#include <iostream>
using namespace std;

int main()  
{
    int n, i, j, k=0, s, count=0, count1=0;
    
    cin>>n;
    
    for(i=1; i<=n; i++)
    {
        for(s=1; s<=n-i; s++)
        {
            cout<<" ";
            count++;
        }
        while(k!=2*i-1)
        {
            if(count<=n-1)
            {
                cout<<k+i;
                count++;
            }
            else
            {
                count1++;
                cout<<i+k-2*count1;
            }
            k++;
        }
        count1 = count = k = 0;
        cout<<endl;
    }   
    return 0;
}  
