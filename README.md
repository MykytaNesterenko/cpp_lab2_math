# cpp_lab2_math
Лабораторна робота №2 — Математичні обчислення на мові C++ (Варіант 25)
#include <iostream>
using namespace std;

int main() {
    cout << "Завдання 1. Integer42\n";

    int P, N;
    cout << "Введіть ціну товару P = ";
    cin >> P;
    cout << "Введіть кількість грошей N = ";
    cin >> N;

    int count = N / P;
    int remain = N % P;

    cout << "Кількість товарів, які можна купити: " << count << endl;
    cout << "Грошей залишиться: " << remain << " грн\n";

    return 0;
}

#include <iostream>
using namespace std;

int main() {
    cout << "Завдання 2. Boolean20\n";

    int num;
    cout << "Введіть тризначне число: ";
    cin >> num;

    int a = num / 100;
    int b = (num / 10) % 10;
    int c = num % 10;

    bool all_diff = (a != b) && (a != c) && (b != c);
    cout << "Всі цифри різні: " << boolalpha << all_diff << endl;

    return 0;
}

#include <iostream>
#include <cmath>
using namespace std;

int main() {
    cout << "Завдання 3. Math.25\n";
    const double pi = 3.141592653589793;

    double x;
    cout << "Введіть значення x = ";
    cin >> x;

    double numerator = pow(pow(x, 6), 1.0 / 5) + sqrt(2 * fabs(x));
    double denominator = log(pow(sin((fabs(2 * x) + 29) * pi / 180), 2)) / log(3);
    double y = numerator / denominator + (pi * fabs(3 * tan(pow(x, 2)))) / 5;

    cout << "Результат y = " << y << endl;
    return 0;
}
