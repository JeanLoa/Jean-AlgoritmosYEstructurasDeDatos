#include <iostream>

using namespace std;

int main() {

	int n = 100;
	int* A = new int[n];

	for (int i = 0; i < n; ++i) {
		A[i] = rand() % 100;
	}

	// Ordenamiento por Selección (Mayor a menor)

	for (int i = 0; i < n; ++i) {
		int maxIdx = i;
		for (int j = i + 1; j < n - 1; ++j) {
			if (A[j] >= A[maxIdx]) {
				maxIdx = j;
			}
		}
		swap(A[i], A[maxIdx]);
	}

	return 0;
}
