# btm1



#include <iostream.h>
#include <math.h>
int main()
{
	double x, y, f, a, s;
	int k;
	cout << "Vvedite x "; cin >> x;
	cout << "Vvedite y "; cin >> y;
	cout << "Viberite f: 1 - sh(x), 2 - x^2, 3 – exp(x) "; cin >> k;
	switch (k)
	{
	case 1: f = sinh(x); break;
	case 2: f = pow(x, 1/3.); break;
	case 3: f = exp(x); break;
	default: cout << "Ne vuibrana funkciya "; return 1;
	}
	a = (x * y);
	        if (a <= 10 && a > 0.5) s = exp(f - fabs(y));
		else
			if (a <= 0.5 && a > 0.1) s = pow(fabs(f+y),1/3.);
			else s = 2*pow(f,2);
	cout << "RESULT = " << s << endl;
	return 0;
}
