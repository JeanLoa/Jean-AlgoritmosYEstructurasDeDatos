#include <iostream>

using namespace std;

int main() {
	int n1 = 5, n2 = 20;
	int** a = new int*[n1];
	for (int i = 0; i < n1; ++i) {
		a[i] = new int[n2];
	}

	for (int i = 0; i < n1; ++i) {
		for (int j = 0; j < n2; ++j) {
			a[i][j] = rand() % 100;
		}
	}

	int** b = new int* [n1] { *(a), *(a + 1), *(a + 2), *(a + 3), *(a + 4) };

	for (int i = 0; i < n1; ++i) {
		for (int j = 0; j < n2; ++j) {
			cout << b[i][j] << " ";
		}
		cout << endl;
	}

	b[0] = *(a);
	b[1] = *(a + 1);
	b[2] = *(a + 2);
	b[3] = *(a + 3);
	b[4] = *(a + 4);

	for (int i = 0; i < n1; ++i) {
		for (int j = 0; j < n2; ++j) {
			cout << b[i][j] << " ";
		}
		cout << endl;
	}

	b[0] = a[0];
	b[1] = a[1];
	b[2] = a[2];
	b[3] = a[3];
	b[4] = a[4];

	for (int i = 0; i < n1; ++i) {
		for (int j = 0; j < n2; ++j) {
			cout << b[i][j] << " ";
		}
		cout << endl;
	}

	for (int i = 0; i < n1; ++i) {
		for (int j = 0; j < n2; ++j) {
			a[i][j] = rand() % 100;
			cout << b[i][j] << " ";
		}
		cout << endl;
	}

	return 0;
}
