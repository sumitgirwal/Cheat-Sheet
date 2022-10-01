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
##### 6. Always use string to input digits
```cpp
#include <iostream>
#include <string>
using namespace std;

int32_t main() {
    int t; cin >> t;
    while (t--) {
		int d; string n; 
		cin>>d; cin>>n;  
		bool flag=false;
		for(int i=0;i<d;i++){	
			if(n[i]=='5' ||n[i]=='0')
			{ flag=true;
				break;
			}
		}		
		if(flag) cout<<"YES"<<endl;
		else cout<<"NO"<<endl;	
    }
    return 0;
}
```

###### long long
```bash
#include <iostream>
#include <vector>
using namespace std;
#define ll long long
#define int ll
int32_t main() {
    int t; cin >> t;
    while (t--) {
			int n; cin>>n;
			vector<int> a(n);
			for(int i=0;i<n;i++) cin>>a[i];
			int count=0;
			int temp=0;
			for(int i=0;i<n;i++){
				int x; cin>>x;
				if(x<=(a[i]-temp)) count++;
				temp = a[i];
			}
			cout<<count<<endl;
    }
    return 0;
}

```

Input:
    string bin_string = "10101010";

    Function call:
    stoi(bin_string, 0, 2);

    Output:
    170
