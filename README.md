# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br>Nama		: Onixa Shafa Putri Wibowo
<br>NIM		        : 1227050107
<br>Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
<br>Pada Source Code ini terdapat 2 Program, yaitu Program Transpose Matrix dan Program Bilangan yang habis dibagi 3,5 dan 7. 
Program Transpose Matrix dibuat dengan cara mengubah/menukar for dan cout "mat" pada saat akan menampilkan output terakhir, sedangkan program kedua dibuat dengan system check menggunakan if else.
Dimana inputan nilai jika habis dibagi angka 3,5, dan 7 berarti angka tersebut benar, sedangkan jika tidak bisa dibagi dengan angka 3,5, dan 7 berarti bukan angka yang dimaksud.
## Source Code
<br> 1. Program Transpose Matrix pada c++:

#include<iostream>
using namespace std;

main(){
	int mat[100][100];
	int i,j, baris, kolom;
  
    cout << "==================================================="<<endl;
    cout << "	Transpose Matrix "<<endl;
  	cout << "===================================================\n"<<endl;
	cout << " Masukkan jumlah baris: ";
	cin >> baris;
	cout << " Masukkan jumlah kolom: ";
	cin >> kolom;
	cout << endl;
	
	for (i = 0; i < baris; i++){
		for (j = 0; j < kolom; j++){
			cout <<" A["<<i+1<<"."<<j+1<<"] : ";
 			cin >> mat[i][j];
			 }
 		cout << endl;
	}
	
	cout << " Hasil: " << endl;
	
	for (i = 0; i < baris; i++){
		for (j = 0; j < kolom; j++){
			cout << "   " << mat[i][j] << " "; 
		}
		cout << endl;
	}
	
	cout << "\n Transpose: " << endl;
	
	for (i = 0; i < kolom; i++){
		for (j = 0; j < baris; j++){
			cout << "   " << mat[j][i] << " "; 
		}
		cout << endl;
	}
  return 0;
 }
  
<br> 2. Program Bilangan yang habis dibagi 3,5, dan 7 pada c++:
  
  #include<iostream>
  using namespace std;

main(){
  	int mat[100][100];
  	int a, k, baris, kolom;
  	
  	cout << "==================================================="<<endl;
    cout << " Memastikan bilangan yang habis dibagi 3,5 dan 7 "<<endl;
  	cout << "===================================================\n"<<endl;
  	cout << " Masukkan jumlah baris: ";
	cin >> baris;
	cout << " Masukkan jumlah kolom: ";
	cin >> kolom;
  	
  	for (a = 0; a < baris; a++)
 	for (k = 0; k < kolom; k++)
 	{
 	cout << " A["<<k+1<<"."<<a+1<<"]: ";
 	cin >> mat[a][k];
 	}
 	
 	for (a = 0; a < baris; a++){
 		for (k = 0; k < kolom; k++){
 			if(mat[a][k]%3 == 0 && mat[a][k]%5 == 0 && mat[a][k]%7 == 0){
  				cout << mat[a][k] << " adalah nilai yang habis dibagi dengan 3, 5 dan 7"<<endl;
  				break;
			  }
			else{
				cout << mat[a][k] << " adalah nilai yang tidak habis dibagi dengan 3, 5 dan 7"<<endl;
				break;
			}
	 }
	}
 	cout << endl;
 	return 0;
}
## Output
<br> Berikut adalah output kedua program tersebut
<br>1. Program Transpose Matrix
![Screenshot 2022-12-27 000308](https://user-images.githubusercontent.com/119369695/209570038-2987acd5-333d-4524-831b-e48b03758175.png)
<br>2. Program Bilangan yang habis dibagi 3,5, dan 7
![Screenshot 2022-12-26 235615](https://user-images.githubusercontent.com/119369695/209569615-92791bf1-a8dc-4d36-a277-f319bab15842.png)
