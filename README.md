# Cheat-Sheet
CPP Cheat Sheet for CP

#### 1. 10^9 long long
#### 2. Sum of 1 to n even & odd numbers
```bash
Sum of even : (n*n)
Sum of odd : (n*(n+1))
```

#### 3. Find sum of all pair in array
```bash
Using map : ans += (i.second*(i.second - 1))/2;
```
#### 4.
#### 5.Small fact
```cpp
// We have populated the solutions for the 10 easiest problems for your support.
// Click on the SUBMIT button to make a submission to this problem.

#include <bits/stdc++.h>
#include <boost/multiprecision/cpp_int.hpp>
#include <iostream>
using namespace std;
using namespace boost::multiprecision;

int main() {
	// your code goes here
	int t;
	cin>>t;
	while(t--)
	{
	    int n;
	    cin>>n;
	    cpp_int fact=1;
	    for(int i=n;i>0;i--)
	     fact=fact*i;
	    cout<<fact<<endl; 
	}
	
	return 0;
}
```



