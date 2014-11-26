PPK
===
CIĄG ARYTMETYCZNY :

REKURENCJA:
long long aryt(int a1, int n, int r)
{
         if(n == 1) return a1 ;
         else return aryt( a1, n-1 , r )+r ;
}

ITERACJA:
wynik = a1 + (n-1) * r;


CIĄG GEOMETRYCZNY :

REKURENCJA:
long long geo(int a1, int n, int q)
{
         if(n == 1) return a1 ;
         else return geo( a1, n-1 , q )*q ;
}

ITERACJA:
wynik = a1 * q ^ (n - 1)


CIĄG FIBONACCIEGO :

REKURENCJA:
int fib(int f)
{
    if ((f==1)||(f==2)) return 1;
    else return fib(f-1)+fib(f-2);
}

ITERACJA:
 fib[0]=1;
    fib[1]=1;
    for (i=2; i<n; i++)
    {
        fib[i]=fib[i-1]+fib[i-2];
    }
    for (i=0; i<n; i++)
    {
        cout << "Wyraz nr " << i+1 << " to: " << fib[i] << endl;
    }


POTEGOWANIE :

REKURENCJA:
int potega(int x, int y)
{
    if (y==0) return 1;
    else return x*potega(x,y-1);
}

ITERACJA:
long int potega(long int podstawa, int wykladnik)
{
    int wynik = 1;
 
    for (int i = 0; i<wykladnik; i++)
        wynik*=podstawa;
 
    return wynik;
}


SILNIA:

REKURENCJA:
long int silnia(int n)
{
    if (n==0) return 1;
    else return n*silnia(n-1);
}

ITERACJA:
 long sil=1;
 for (int i=1; i<=x; i++) 
{ 
    sil=i*sil;
}
