# praktikum6

##latihan1.cpp : Buatlah fungsi(void) menggunakan passing parameter by reference untuk menukar nilai dari dua buah variable.

**Alur algoritma**
1. Mendeklarasikan variabel 'int(kali, bagi, tambah, kurang);' sebagai variable input.
2. Membaca input dari keyboard 'return a*b, a/b, a+b, a-b'
3. Membandingkan nilai variable return a*b, a/b, a+b, a-b

**Flowchart Program**
![Flowchart](https://raw.githubusercontent.com/tedyajadeh/praktikum6/master/Flowchart1.png)

**Screenshoot**
![Screenshoot](https://raw.githubusercontent.com/tedyajadeh/praktikum6/master/Screenshot1.png)

**code program lengkap**
'''c++
#include<iostream>
using namespace std;

int kali(int a, int b){
return a*b;
}

double bagi(int a, int b){
return a/b;
}

int tambah(int a, int b){
return a+b;
}

int kurang(int a, int b){
return a-b;
}



###latihan2.cpp :  Buatlah fungsi perkalian 2 buah bilangan bulat dengan menggunakan operator penjumlahan. (gunakan passing by value)

**Alur algoritma**
1. Mendeklarasikan variabel 'void tukar(int *a, int *b)' sebagai variable input.
2. Membaca input dari keyboard 'int c;
    				c = *a;
    				*a = *b;
    				*b = c;'
3. Membandingkan nilai variable  cout << "Nilai 1 : " << a << endl;
				 cout << "Nilai 2 : " << b << endl;


**Flowchart Program**
![Flowchart21](https://raw.githubusercontent.com/tedyajadeh/praktikum6/master/Flowchart21.png)

**Flowchart Program**
![Flowchart22](https://raw.githubusercontent.com/tedyajadeh/praktikum6/master/Flowchart22.png)

**Screenshoot**
![Screenshoot21](https://raw.githubusercontent.com/tedyajadeh/praktikum6/master/Screenshoot21.png)

**Screenshoot**
![Screenshoot22](https://raw.githubusercontent.com/tedyajadeh/praktikum6/master/Screnshoot22.png)

**code program lengkap**
'''c++
#include<iostream>
using namespace std;

void tukar(int *a, int *b)
{
    int c;
    c = *a;
    *a = *b;
    *b = c;

}
main(){
int a = 5, b = 8;
cout<< "\nSebelum di tukar\n";
cout << "Nilai 1 : " << a << endl;
cout << "Nilai 2 : " << b << endl;
tukar(&a, &b);
cout << "\nSesudah ditukar\n";
cout << "Nilai 1 : " << a << endl;
cout << "Nilai 2 : " << b << endl;
return 0;
}
