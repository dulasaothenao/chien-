# chien-#include <conio.h>
#include <stdio.h>
#include <iostream.h>

int d;
void chuyen(int, char, char, char);
void chuyen(int n, char a, char b, char c)
{
	if (n == 1) cout << "\nLan chuyen " << ++d << " : Tu " << a << " sang " << b;
	else
	{
		chuyen(n - 1, a, c, b);
		chuyen(1, a, b, c);
		chuyen(n - 1, c, b, a);
	}
}#include <conio.h>
#include <stdio.h>
#include <iostream.h>

int d;
void chuyen(int, char, char, char);
void main()
{
	int n;
	char c;
	do {
		cin >> c;
	} while ((c == 'c') || (c == 'C'));
}

void chuyen(int n, char a, char b, char c)
{
	if (n == 1) cout << "\nLan chuyen " << ++d << " : Tu " << a << " sang " << b;
	else
	{
		chuyen(n - 1, a, c, b);
		chuyen(1, a, b, c);
		chuyen(n - 1, c, b, a);
	}
}
