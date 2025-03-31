#include <iostream>

using namespace std;

int main() {

	int n = 100;
	int* A = new int[n];

	int maxIdx = 0;

	for (int i = 0; i < n; ++i) {
		A[i] = rand() % 100;
		if (A[maxIdx] <= A[i]) {
			maxIdx = i;
		}
	}

	cout << "El maximo valor tiene indice de " << maxIdx << " con un valor de: " << A[maxIdx];

	return 0;
}
