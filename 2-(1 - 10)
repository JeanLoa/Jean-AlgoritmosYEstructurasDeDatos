#include <iostream>
#include <vector>
#include <string>

using namespace std;

int main() {
	// 1
	auto lambda1 = []() {
		double a, b, c;
		cout << "Ingrese a - b - c: ";
		cin >> a >> b >> c;


		double a_ = sqrt(a);
		double b_ = sqrt(b);
		double c_ = sqrt(c);

		int sum = a_ + b_ + c_;
		cout << "Suma de sus raices cuadradas: " << sum;
		system("pause>0");
		system("cls");
		};

	lambda1();

	// 2
	auto lambda2 = []() {
		int a, b, c, d, e;
		cout << "Ingrese a - b - c - d - e: ";
		cin >> a >> b >> c >> d >> e;

		int min = a;
		if (b <= min) {
			min = b;
		}
		else if (c <= min) {
			min = c;
		}
		else if (d <= min) {
			min = d;
		}
		else if (e <= min) {
			min = e;
		}
		cout << "El minimo es: " << min;
		system("pause>0");
		system("cls");
		};

	lambda2();

	// 3
	auto lambda3 = []() {
		int a, b, c;
		cout << "Ingrese a - b - c: ";
		cin >> a >> b >> c;

		int sum = a + b + c;

		if (sum % 3 == 0) cout << "El numero " << sum << " es multiplo de 3";
		else cout << "El numero " << sum << " no es multiplo de 3";

		system("pause>0");
		system("cls");
		};

	lambda3();

	// 4
	auto lambda4 = []() {
		int a, b, c;
		cout << "Ingrese a - b - c: ";
		cin >> a >> b >> c;

		int max = a;
		if (b >= max) {
			max = b;
		}
		if (c >= max) {
			max = c;
		}
		cout << "El maximo es: " << max;
		system("pause>0");
		system("cls");
		};

	lambda4();

	// 5
	auto lambda5 = []() {
		char a;
		cout << "Ingrese una letra o numero: ";
		cin >> a;

		if ((a >= 'A' && a <= 'Z') || (a >= 'a' && a <= 'z')) {
			cout << "Es una letra";
		}
		else {
			cout << "Es un numero";
		}
		system("pause>0");
		system("cls");
	};
	lambda5();

	// 6
	auto lambda6 = []() {
		float a, b, c;
		cout << "Ingrese a - b - c: ";
		cin >> a >> b >> c;

		if (a == b && b == c) cout << "Los 3 numeros son iguales";
		else cout << "Los 3 numeros no son iguales";

		system("pause>0");
		system("cls");
	};
	lambda6();

	// 7
	auto lambda7 = []() {
		int a;
		cout << "Ingrese un numero de 5 digitos: ";
		cin >> a;

		int a_ = a;

		int num = 0;
		int i = 0;
		while (a_ > 0) {
			if (i == 2) num = a_ % 10;
			a_ /= 10;
			++i;
		}
		if (i != 5) {
			cout << "El numero no tiene 5 digitos";
			system("pause>0");
			system("cls");
			return;
		}

		if (num % 2 == 0) cout << "El numero del centro de " << a << " es par";
		else cout << "El numero del centro de " << a << " es impar";

		system("pause>0");
		system("cls");
	};

	lambda7();

	// 8
	auto lambda8 = []() {
		int a, b;
		cout << "Ingrese a - b: ";
		cin >> a >> b;

		int sum = a + b;

		if (sum % 3 == 0) cout << "El numero " << sum << " es multiplo de 3";
		else cout << "El numero " << sum << " no es multiplo de 3";

		system("pause>0");
		system("cls");
	};

	lambda8();

	// 9
	auto lambda9 = []() {
		string a;
		cout << "Ingrese un numero: ";
		cin >> a;

		int lenght = a.size();
		vector<int> l(lenght), r(2);
		
		int a_ = stoi(a);
		int i = 0;
		int j = 0, k = 0;

		while (a_ > 0) {
			int res = a_ % 10;
			if (a_ > 100) {
				l[j] = res;
				j++;
			}
			else if (a_ > 0) {
				r[k] = res;
				k++;
			}
			a_ /= 10;
			++i;
		}
		int numL = l[0] * 10 + l[1];
		int numR = r[0] * 10 + r[1];
		if (i != 4) {
			cout << "El numero no tiene 4 digitos";
			system("pause>0");
			system("cls");
			return 1;
		}

		if (numL > 50) cout << "El numero izquierdo es mayor a 50";
		else cout << "El numero izquierdo no es mayor a 50";
		cout << endl;

		if (numR % 2 != 0) cout << "El numero derecho es impar";
		else cout << "El numero derecho no es impar";

		system("pause>0");
		system("cls");
	};

	lambda9();

	// 10
	auto lambda10 = [](int* a, int n, bool asc, bool (orden)(int a, int b, bool asc)) {
		for (int i = 0; i < n; ++i) {
			for (int j = 0; j < n - i - 1; ++j) {
				if (orden(a[j], a[j + 1], asc)) {
					swap(a[j], a[j + 1]);
				}
			}
		}

		for (int i = 0; i < n; ++i) {
			cout << a[i] << " ";
		}

		system("pause>0");
		system("cls");
	};

	auto lambda_aux = [](int a, int b, bool asc) {
		if (asc) {
			if (a > b) return true;
			else return false;
		}
		else {
			if (a < b) return true;
			else return false;
		}
	};

	int* a = new int[10];
	for (int i = 0; i < 10; ++i) {
		a[i] = rand() % 20;
	}
	lambda10(a, 10, false, lambda_aux);

	return 0;
}
