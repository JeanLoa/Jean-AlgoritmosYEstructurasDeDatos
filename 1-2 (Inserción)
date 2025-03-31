#include <iostream>

using namespace std;

int main() {

	int n = 100;
	int* A = new int[n];

	for (int i = 0; i < n; ++i) {
		A[i] = rand() % 100;
	}

	// Ordenamiento por Inserción (Menor a mayor)

	for (int i = 1; i < n; ++i) {
		
		int key = A[i];
		int j = i - 1;
		
		while (j >= 0 && key <= A[j]) {
			A[j + 1] = A[j];
			--j;
		}

		key = A[j + 1];
	}

	return 0;
}
