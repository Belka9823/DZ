## репозиторий для предметов Летунова Ильи Анатольевича

### [ Архитектура Аппаратных средств ](/Архитектура_Аппаратных_средств)
### [ Внедрение и поддержка комп.систем ](/Внедрение_и_поддержка_комп.систем)

жизненый цикл программы/системы - ЗАПОМНИ!!!
утилиты определение конфигурации ПК

// ConsoleApplication1.cpp : Этот файл содержит функцию "main". Здесь начинается и заканчивается выполнение программы.
//

#include <iostream>
#include <iomanip>
	using namespace std;

int main()
{
	setlocale(LC_ALL, "Ru");

	string BibleS[30] = { "0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T" };
	int KeyB;
	string Answer;
	int numA;
	int numB;
	int A = 1;
	int B = 1;

	cout << "Введите первое число:";
	cin >> numA;
	cout << "Введите второе число:";
	cin >> numB;
	KeyB = numA + numB;
	

	if (KeyB > 29)
	{
		A = KeyB % 30;
		KeyB -= 30;
	    Answer = BibleS[B] + BibleS[A];
		B++;
	}
	else
	{
		Answer = BibleS[KeyB];
	}
	cout << "Ответ в тридцатизначной системе: " << Answer;

	return 0;
}







