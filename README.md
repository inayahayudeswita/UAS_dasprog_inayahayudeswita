# UAS_dasprog_inayahayudeswita
# Ujian Akhir Semester 
<br>Mata Kuliah  : Dasar Pemrograman
<br> Nama  : Inayah Ayu Deswita
<br>NIM  : 1227050058
<br>Jurusan  :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

## Source Code 
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

## Output
