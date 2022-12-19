# UAS_dasprog_inayahayudeswita
# Ujian Akhir Semester 
<br>Mata Kuliah  : Dasar Pemrograman
<br> Nama  : Inayah Ayu Deswita
<br>NIM  : 1227050058
<br>Jurusan  :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

Pengertian yang bisa dijelaskan secara singkat mengenai matriks adalah bilangan-bilangan yang diatur pada sebuah baris dan juga kolom. Anggota dalam bilangan-bilangan yang terdapat di dalam formasi mencatat disebutkan sebagai baris, dan formasi sekumpulan bilangan yang dicatat secara menurun disebut sebagai kolom. 

Matriks Transpose adalah suatu matriks yang dikerjakan pertukaran antara dimensi kolom dan baris. Definisi lain dari transpose matriks tersebut adalah sebuah matriks yang didapatkan dengan cara memindahkan elemen – elemen pada sebuah kolom menjadi elemen – elemen sebuah baris dan sebaliknya.

## Source Code 
```
1. Program Transpose

        #include <iostream>
        using namespace std;

        int main(void)
        {
          system("Color B");
          cout<<endl;
          cout<<"Nama : Inayah Ayu Deswita"<<endl;
          cout<<"NIM  : 1227050058"<<endl;
          cout << "===============================" << endl;
          cout << "|| Program Matriks Transpose ||" << endl;
          cout << "===============================" << endl;
          cout << endl;
            #
          int i, j, m, n, matriks[10][10], transpose[10][10];

          cout << "Masukkan jumlah baris matriks: ";
          cin >> m;
          cout << "Masukkan jumlah kolom matriks: ";
          cin >> n;

          cout << "Masukkan elemen matriks\n";
          for (i = 0; i < m; i++){
            for (j = 0; j < n; j++){
              cin  >> matriks[i][j];
            }
          }

          for (i = 0; i < m; i++){
            for (j = 0; j < n; j++){
              transpose[j][i] = matriks[i][j];
            }
          }

          cout<<"Gambar Matriks\n";
          for (i = 0; i < m; i++){
            for (j = 0; j < n; j++){
              cout << transpose[j][i] << "\t";
            }
            cout << endl;
          }


          cout << "Hasil Transpose Matriks: \n";
          for (i = 0; i < n; i++){
            for (j = 0; j < m; j++){
              cout << transpose[i][j] << "\t";
            }
            cout << endl;
          }
        }
	```
2. Program elemen matriks yang bisa dibagi 3,5,7
```

                #include <iostream>
                #include <iomanip>
                using namespace std;
                int main(){

                system("Color D");
                cout<<endl;
                cout<<" Nama	: Inayah ayu deswita"<<endl;
                cout<<" NIM	: 1227050058"<<endl;
                cout<<" ================================ "<<endl<<endl;

		int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;
	
	    cout<<" Input jumlah baris: "; cin>>jumlahBaris;
	    cout<<" Input jumlah kolom: "; cin>>jumlahKolom;
	    cout << endl;
	
	    for(i = 0; i < jumlahBaris; i++){
	        for(j = 0; j < jumlahKolom; j++){
	            cout << " Baris " <<i+1<<", kolom "<<j+1<< " = ";
	            cin >> arr[i][j];
	        }
	        cout << endl;
	    }
	
	    cout << " Hasil input nilai : " << endl;
	
	    for(i = 0; i < jumlahBaris ; i++){
	    for(j = 0; j < jumlahKolom; j++){
	        cout << setw(3) << arr[i][j] << " ";
	    }
	    cout << endl;
	    }
	
	    cout << "\n Hasil bilangan yang bisa dibagi 3,5,7 : " << endl;
	
	    for(i = 0; i < jumlahBaris ; i++){
	    for(j = 0; j < jumlahKolom; j++){
	        if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
	        cout << setw(3) << arr[i][j] << " ";
	        }
	    }
	    cout << endl;
	    }

    cout << endl;

    return 0;
}

## Output
1. Pogram Transpose

        
<img width="960" alt="Screenshot_20221219_043436" src="https://user-images.githubusercontent.com/121011237/208394930-3b735fd4-ecfd-4d32-a206-51243a342045.png">

        
2. Program Elemen Matriks yang Bisa Dibagi 3,5,7

	  
	  <img width="866" alt="Screenshot_20221219_043523" src="https://user-images.githubusercontent.com/121011237/208394288-8678394e-8361-43ce-9eac-dfce08ab1618.png">

