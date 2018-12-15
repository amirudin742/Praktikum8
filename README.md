# Praktikum8

#latihan1#Fibonanci dengan fungsi iteratif

1. Alur Algoritmanya

	-mendefinisikan fungsi fibonanci

	int fibonanci (int suku, int a, int b, int c)

-mengisi int a =0 dan int b=1

-membuat rumus if untuk perbandingan dan rumus fibonanci

```c++
 if (suku== 1) //jika nilai suku 1,nilai=1
        return b;
    if (suku==0)//jika nilai suku 0,nilai=0
        return a;
    else
        {
        for ( int i=2; i<=suku; i++){
            c=a+b; //suku ke-3 = suku kw-1 + suku ke-2
            a=b;//nilai suku a diisi dengan n
            b=c;//nilai suku b disi dengan nilai suku c
        }
        return c;```

Berikut kode lengkapnya

```#include <iostream>

using namespace std;
int fibonanci (int suku, int a, int b, int c)
{
    a=0; //int nilai a 0
    b=1;// int nilai b 1
    if (suku== 1) //jika nilai suku 1,nilai=1
        return b;
    if (suku==0)//jika nilai suku 0,nilai=0
        return a;
    else
        {
        for ( int i=2; i<=suku; i++){
            c=a+b; //suku ke-3 = suku kw-1 + suku ke-2
            a=b;//nilai suku a diisi dengan n
            b=c;//nilai suku b disi dengan nilai suku c
        }
        return c;
        }
}
int main()
{
    int suku,a,b,c;

    cout << "Masukan nilai suku Ke-: " ;
    cin>> suku;
    cout<<"\n Bilangan Fibonanci untuk "<< suku << " Adalah ";
    cout<< fibonanci(suku,a,b,c);
    return 0;
}```

Berikut adalah flowchartnya

![img](https://raw.githubusercontent.com/amirudin742/Praktikum8/master/Flowchart1.png)

Berikut adalah hasilnya

![img](https://raw.githubusercontent.com/amirudin742/Praktikum8/master/Hasil1.png)

