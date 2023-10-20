#include <iostream>
#include <cstdlib>
#include <ctime>
#include <wchar.h>
#include <Windows.h>
#include <algorithm>
#include <vector>
#include <string>
#include <cstring>
#include <conio.h>
#include <iomanip>

using namespace std;



int main()
{
    string aName = "Ivan";
    string userName;
    cout << "Enter your name: ";
    cin >> userName;
    if (userName == aName) {
        cout << "Hello, Ivan\n";
    }
    else if (userName < aName) {
        cout << "Your name goes before the name Ivan\n";
    }
    else {
        cout << "Your name comes after the name Ivan\n";
    }

    int n = userName.compare(0, 2, aName, 0, 2);
    cout << "The first two letters of your name: ";
    if (n == 0)
        cout << "match ";
    else if (n < 0)
        cout << "go to ";
    else
        cout << "go after ";

    cout << aName.substr(0, 2) << endl;
 


    return 0;
}
