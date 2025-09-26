#include <iostream>
using namespace std;

int main() {
    int n;
    long long fact = 1;   // long long to handle large values

    cout << "Enter a positive integer: ";
    cin >> n;

    if (n < 0) {
        cout << "Factorial is not defined for negative numbers." << endl;
    } else {
        for (int i = 1; i <= n; i++) {
            fact *= i;   // fact = fact * i
        }
        cout << "Factorial of " << n << " is: " << fact << endl;
    }

    return 0;
}
