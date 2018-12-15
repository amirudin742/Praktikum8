# Praktikum8

#latihan1#Fibonanci dengan fungsi iteratif

1. Alur Algoritmanya

	-mendefinisikan fungsi fibonanci

	int fibonanci (int suku, int a, int b, int c)

	-mengisi int a =0 dan int b=1

	-membuat rumus if untuk perbandingan dan rumus fibonanci

 c++
 
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

2 Berikut adalah kodenya

#include <iostream>

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
}

3 Berikut adalah flowchartnya

![img](https://raw.githubusercontent.com/amirudin742/Praktikum8/master/Flowchart1.png)

4 Berikut adalah hasilnya

![img](https://raw.githubusercontent.com/amirudin742/Praktikum8/master/Hasil1.png)

#Latihan2#Perkalian dengan penjumlahan menggunakan fungsi rekursif

1.Alur Algoritmanya
	-Mendefinisikan fungsi kali
int kali (int a, int b)
	-membuat rumus if dan perkalianya
if (b==0) //jika nilai b=0 maka hasilnya 0
        return 0;
    else
        return a+kali(a,b-1); // nilai a ditambah (nilai a ditambah nilai b dikurangi 1)
2.Berikut kode lengkapnya

#include <iostream>

using namespace std;
int kali (int a, int b)
{
    if (b==0)
        return 0;
    else
        return a+kali(a,b-1);
        cout<< a;
}
int main()
{
    int a,b;
    cout << "Masukan bilangan pertama :";
    cin>> a;
    cout << "Masukan bilangan kedua :";
    cin>> b;
    cout<< " Hasil = " <<kali (a,b);
    return 0;
}
3.Berikut flowchartnya

![img](https://raw.githubusercontent.com/amirudin742/Praktikum8/master/Flowchart2.png)

4.Berikt adalah hasilya

![img](https://raw.githubusercontent.com/amirudin742/Praktikum8/master/Hasil2.png)