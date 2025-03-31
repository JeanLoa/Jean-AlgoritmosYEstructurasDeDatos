#include <iostream>

using namespace std;

int main() {
	int n = 100;
	int* A = new int[n];

	for (int i = 0; i < n; ++i) {
		A[i] = rand() % 100;
	}

	// Ordenamiento por Burbuja (Menor a mayor)

	for (int i = 0; i < n; ++i) {
		for (int j = 0; j < n - i - 1; ++j) {
			if (A[j] >= A[j + 1]) {
				swap(A[j], A[j + 1]);
			}
		}
	}
	return 0;
}
