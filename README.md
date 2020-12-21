# Arrays
#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;



    /* Enter your code here. Read input from STDIN. Print output to STDOUT */  

void print(int arr[], int n)
{
	for (int i = 0; i < n; i++) {
		cout << arr[i] << " ";
	}
}
void reverse(int arr[], int n)
{
	reverse(arr, arr + n);
}



int main()
{
    int s;
    cin >> s;
	int arr[s];
    for(int k = 0; k < s; ++k )
    {
        cin>>arr[k];
    }
	int n = sizeof(arr)/sizeof(arr[0]);
	reverse(arr, n);
	print(arr, n);

	return 0;
}
