#include <iostream>

using namespace std;

bool esPrimo(int num) {
	if (num <= 1) return false;

	for (int i = 2; i <= sqrt(num); ++i) {
		if (num % i == 0) {
			return false;
		}
	}

	return true;
}

int main() {
	int n = 100;
	int* arr = new int[n];

	int nPrimos = 0;

	for (int i = 0; i < n; ++i) {
		arr[i] = rand() % 100;
		if (esPrimo(arr[i])) ++nPrimos;
	}

	cout << "La cantidad de numeros primos en el arreglo dinamico aleatorio es: " << nPrimos;

	return 0;
}
