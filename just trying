#include <sstream>
#include <vector>
#include <iostream>
using namespace std;

vector<int> parseInts(string str) 
{	
    str = str + ",";
	vector<int> numbers;
    long int n = str.size();
    int a = 0;
    int x = 0;
    for (int i=0; i<n; i++) 
    {
        if(str[i] != ',')
        {
        	sscanf(str[i], "%d", &x);
            a = a*10 + str[i] - '0';
        }
        else
        {
            numbers.push_back(a);
            a = 0;
        }
    }
    return numbers;
}

int main() 
{
    string str;
    cin >> str;
    vector<int> integers = parseInts(str);
    for(int i = 0; i < integers.size(); i++) 
    {
        cout << integers[i] << "\n";
    }
    
    return 0;
}
