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
2. Program elemen matriks yang bisa dibagi 3,5,7

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

        Nama : Inayah Ayu Deswita
        NIM  : 1227050058
        ===============================
        || Program Matriks Transpose ||
        ===============================

        Masukkan jumlah baris matriks: 3
        Masukkan jumlah kolom matriks: 2
        Masukkan elemen matriks
        2
        34
        5
        43
        3
        23
        Gambar Matriks
        2       34
        5       43
        3       23
        Hasil Transpose Matriks:
        2       5       3
        34      43      23

        --------------------------------
        Process exited after 21.55 seconds with return value 0
        Press any key to continue . . .
        
2. Program Elemen Matriks yang Bisa Dibagi 3,5,7


         Nama   : Inayah ayu deswita
         NIM    : 1227050058
         ================================

         Input jumlah baris: 3
         Input jumlah kolom: 3

         Baris 1, kolom 1 = 23
         Baris 1, kolom 2 = 12
         Baris 1, kolom 3 = 21

         Baris 2, kolom 1 = 21
         Baris 2, kolom 2 = 12
         Baris 2, kolom 3 = 3

         Baris 3, kolom 1 = 23
         Baris 3, kolom 2 = 7
         Baris 3, kolom 3 = 12

         Hasil input nilai :
         23  12  21
         21  12   3
         23   7  12

         Hasil bilangan yang bisa dibagi 3,5,7 :
         12  21
         21  12   3
          7  12
