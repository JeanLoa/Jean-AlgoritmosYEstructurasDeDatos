#include <iostream>
#include <vector>
#include <algorithm>

using namespace std;

int sumaDigitos(int num) {
	int suma = 0;

	while (num > 0) {
		suma += num % 10;
		num /= 10;
	}

	return suma;
}

int main() {

	int num = 12345;
	cout << sumaDigitos(num);

	return 0;
}
