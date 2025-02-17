## JOBSHEET 7

## PERULANGAN 1

### Tujuan

Mahasiswa mampu menyelesaikan permasalahan/studi kasus menggunakan sintaks perulangan 1 dan mengimplemantasikannya dalam bahasa pemrogaman java.

### Alat dan Bahan
+ PC/laptop
+ Browser(chrome, firefox, safari)
+ Koneksi internet

### Praktikum

#### Percobaan 1 : Penggunaan for, while dan do-while

#### Waktu percobaan : 40 menit

1. Perhatikan flowchart perulangan for dibawah ini!

    <p align="left">
    <img width="197" height="259" src="images/flowchartFaktorial.png">
    </p>
    

> Flowchart diatas digunakan untuk menghitung nilai faktorial, selanjutnya kita akan membuat programnya berdasarkan
> flowchart di atas!

2. Tambahkan library Scanner, deklarasi Scanner, dan buat variabel angka untuk menampung data yang diinput melalui keyboard




```Java
// Ketik kode program di bawah sini
import java.util.Scanner;
Scanner input = new Scanner(System.in);
```

3. Buatlah deklarasi dan inisialisasi variabel faktorial sesuai dengan flowchart diatas


```Java
// Ketik kode program di bawah sini
int angka, faktorial = 1;
```

4. Tambahkan struktur perulangan untuk menghitung hasil faktorial sebuah nilai yang diinputkan menggunakan for
    
    <p align="left">
    <img width="696" height="124" src="images/for.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
System.out.println("=====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN FOR=====");
System.out.print("Masukkan Bilangan : ");
angka = input.nextInt();
for(int i=1; i<=angka; i++)
    faktorial*= i;
System.out.print("Nilai faktorial bilangan tersebut adalah : "+ faktorial);
```

    =====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN FOR=====
    Masukkan Bilangan : 5
    Nilai faktorial bilangan tersebut adalah : 120

5. Ubah nilai variabel faktorial seperti semula. Kemudian gunakan struktur perulangan while untuk menghitung hasil faktorial sebuah nilai yang diinputkan
    
    <p align="left">
    <img width="696" height="124" src="images/while.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
faktorial = 1;
System.out.println("=====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN FOR=====");
System.out.print("Masukkan Bilangan : ");
angka = input.nextInt();
int i = 1;
while(i<=angka){
    faktorial*= i;
    i++;
}    
System.out.print("Nilai faktorial bilangan tersebut adalah : "+ faktorial);
```

    =====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN FOR=====
    Masukkan Bilangan : 5
    Nilai faktorial bilangan tersebut adalah : 120

6. Kembalikan lagi nilai variabel faktorial seperti semula. Gunakan struktur perulangan do-while untuk menghitung hasil faktorial sebuah nilai yang diinputkan
    
    <p align="left">
    <img width="696" height="124" src="images/dowhile.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
faktorial = 1;
System.out.println("=====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN FOR=====");
System.out.print("Masukkan Bilangan : ");
angka = input.nextInt();
int i = 1;
do{
    faktorial*= i;
    i++;
}    
while(i<=angka);
System.out.print("Nilai faktorial bilangan tersebut adalah : "+ faktorial);
```

    =====PROGRAM MENGHITUNG NILAI FAKTORIAL DENGAN FOR=====
    Masukkan Bilangan : 5
    Nilai faktorial bilangan tersebut adalah : 120

Program di atas menunjukkan program dengan menggunakan sistem perulangan dan dengan 3 cara yaitu for, while, dan do-while

##### Pertanyaan
1. Pada program diatas, apakah kegunaan baris berikut?
<p align="left">
    <img src="images/hitungFaktorial.jpg" align="left">
    </p>

Jadi maksud dari faktorial*=i sama halnya dengan faktorial = faktorial * i, 
jadi faktorial pertama dikali dengan angka i pertama dan hasilnya akan operasikan kembali 
pada looping yang kedua yaitu hasil dari faktorial pertama dikali dengan i yang kedua 
begitupun seterusnya sampai dengan angka yang dimasukkan/diinputkan.

2. Modifikasi program diatas dibagian struktur pemilihannya sehingga hasilnya menjadi seperti di bawah ini:
<p align="left">
    <img src="images/modifP1.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
import java.util.Scanner;
Scanner input = new Scanner(System.in);

int faktorial = 1, angka;
System.out.println("=====PROGRAM MENGHITUNG NILAI FAKTORIAL=====");
System.out.print("Masukkan Bilangan : ");
angka = input.nextInt();
int i = 1;
System.out.print(angka + " Faktorial = "+ i);

while(i <= angka){
    faktorial*= i;
    i++;
    if(i <= angka)
    System.out.printf("x%d", i);
}
System.out.println(" = " + faktorial);
```

    =====PROGRAM MENGHITUNG NILAI FAKTORIAL=====
    Masukkan Bilangan : 5
    5 Faktorial = 1x2x3x4x5 = 120


#### Percobaan 2 : Keluar dari perulangan menggunakan break

#### Waktu percobaan : 40 menit

1. Buatlah perulangan dengan menggunakan for yang memanfaatkan keyword break
<p align="left">
    <img width="696" height="124" src="images/for2.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
Scanner input = new Scanner(System.in);
int angka,total;
System.out.println("===PROGRAM FOR LOOP DENGAN BREAK");
for(total=0;true;){
    System.out.print("Masukkan Bilangan : ");
    angka=input.nextInt();
    total+=angka;
    if(total>50) break;
}
System.out.println("Jumlah angka-angka yang telah dimasukkan : "+total);
```

    ===PROGRAM FOR LOOP DENGAN BREAK
    Masukkan Bilangan : 1
    Masukkan Bilangan : 2
    Masukkan Bilangan : 3
    Masukkan Bilangan : 4
    Masukkan Bilangan : 5
    Masukkan Bilangan : 6
    Masukkan Bilangan : 7
    Masukkan Bilangan : 8
    Masukkan Bilangan : 9
    Masukkan Bilangan : 10
    Jumlah angka-angka yang telah dimasukkan : 55


2. Buat perulangan yang sama dengan struktur perulangan while
<p align="left">
    <img width="696" height="124" src="images/while2.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
int angka, total;
System.out.println("===POGRAM WHILE LOOP DENGAN BREAK===");
total=0;
while(true){
    System.out.print("Masukkan Bilangan : ");
    angka=input.nextInt();
    total+=angka;
    if(total>50) break;
}
System.out.println("Jumlah angka-angka yang telah dimasukkan : "+total);
```

    ===POGRAM WHILE LOOP DENGAN BREAK===
    Masukkan Bilangan : 2
    Masukkan Bilangan : 4
    Masukkan Bilangan : 6
    Masukkan Bilangan : 8
    Masukkan Bilangan : 10
    Masukkan Bilangan : 12
    Masukkan Bilangan : 14
    Jumlah angka-angka yang telah dimasukkan : 56


3. Tuliskan perulangan diatas dalam struktur do-while
    <p align="left">
    <img width="696" height="124" src="images/dowhile2.jpg" align="left">
    </p>


```Java
// Ketik kode program di atas di bawah sini
int angka, total;
System.out.println("===PROGRAM DO-WHILE LOOP DENGAN BREAK===");
total=0;
do
{
    System.out.print("Masukkan Bilangan  ");
    angka=input.nextInt();
    total+=angka;
    if(total>50) break;
}
while(true);
System.out.println("Jumlah angka-angka yang telah dimasukkan : "+total);
```

    ===PROGRAM DO-WHILE LOOP DENGAN BREAK===
    Masukkan Bilangan  1
    Masukkan Bilangan  3
    Masukkan Bilangan  5
    Masukkan Bilangan  7
    Masukkan Bilangan  9
    Masukkan Bilangan  11
    Masukkan Bilangan  13
    Masukkan Bilangan  15
    Jumlah angka-angka yang telah dimasukkan : 64

Pada percobaan 2 program tersebut menjelaskan penggunaan sistem for, while, dan do-while dengan break. Yang di mana jika output sudah memenuhi syarat atau ekspresi maka proses akan berhenti dan menampilkan output yang sudah dimasukkan

Penjelasan

##### Pertanyaan
1. Jelaskan fungsi kode program yang telah dibuat pada percobaan diatas!

Jadi untuk fungsi kode program pada percobaan 2 melakukan looping 
atau perulangan dengan memasukkan angka di setiap perulangan dengan cara menambahkan perintah break.

2. Jelaskan fungsi kode berikut!
    <p align="left">
    <img src="images/forPertanyaan2.jpg" align="left">
    </p>


total=0 code tersebut untuk kalau masuk ke rumus + angka itu yang muncul angakanya saja dan untuk true itu menunjukkan bagian exp2 karena berisi statement kalau setiap yang diinputkan benar


#### Percobaan 3 : Keluar dari step perulangan menggunakan continue

#### Waktu percobaan : 40 menit

1. Buat program looping menggunakan struktur perulangan for seperti di bawah ini: 
<p align="left">
    <img src="images/forContinue.jpg" align="left">
    </p>



```Java
5. Jalankan program. Amati apa yang terjadi!
```


```Java
Scanner input = new Scanner(System.in);
int angka, total, count;
double avg;
count=0;
System.out.println("===PROGRAM FOR LOOP DENGAN CONTINUE===");
for(int i=0; i<5; i++){
    System.out.print("Masukkan Bilangan : ");
    angka = input.nextInt();
    if(angka>=50) continue;
    total+=angka;
    count++;
}
System.out.println("Jumlah angka-angka yang kurang dari 50: "+total);
avg=(double)total/count;
System.out.println("Rata-rata yang kurang dari 50: "+avg);
```

Pada percobaan 3 menggunakan code program menggunakan statement continue, di mana jika kondisi memenuhi statement continue maka angka tersebut diabaikan dan looping tetap berjalan. Dalam contoh percobaan 3 menampilkan jumlah angka dan rata-rata dari angka yang kurang dari 50.

##### Pertanyaan
1. Jelaskan Perbedaan dari percobaan 2 dan percobaan 3

Perbedaan dari percobaan 2 dan percobaan 3, kalau percobaan 2 itu menggunakan perintah break yang di mana jika kondisi memenuhi dari perintah break maka looping akan berhenti. Sedangkan, untuk percobaan 3 itu menggunakana perintah continue yang di mana jika kondisi looping bertemu continue maka loop akan tetap berjalan dengan mengabaikan hasil dari nilai yang diseleksi pada kondisi continue.

2. Jelaskan apa fungsi perintah kode program dibawah ini?
<p align="left">
    <img width="352" height="79" src="images/continuePertanyaan.jpg" align="left">
    </p>


Fungsi dari perintah code program if(angka>=50) continue; itu yaitu jika angka yang diinput lebih dari sama dengan 50 maka angka tersebut diabaikan dan lanjut ke looping selanjutnya. Dan setiap angka yang memenuhi kondisi pada continue atau kurang dari 50 akan dijumlahkan/ ditotal. Dan untuk count++ merupakan jumalah angka yang dimasukkan tetapi angkanya terhitung jika kurang dari 50


### Tugas

#### Waktu pengerjaan Tugas: 140 menit

1. Buatlah program yang meminta masukan user sebuah bilangan bulat N (N > 0). Program kemudian menampilkan penjumlahan N bilangan genap positif pertama (bilangan genap ≥ 0).
Contoh: 
    •	Jika user memasukkan N = 10, program akan menghitung banyaknya jumlah bilangan positive di dalam range bilangan 1-10   kemudian menampilkan penjumlahan bilangan positive bilangan bilangan diantara 1-10 yaitu : 
        0 + 2 + 4 + 6 + 10 = 30. 
        Setelah itu program akan menampilkan rata-rata dari bilangan positive yang telah dijumlahkan tadi.
    •	Contoh output program dan flowchart
<br/><img width="303" height="529" src="images/hasilTugasFc.jpg" align="left"><br/>
  

<br/><img width="303" height="529" src="images/fcTugasJS7.png" align="left">



```Java
// Ketik kode program disini
import java.util.Scanner;
Scanner input = new Scanner(System.in);
int bil, jmlBilGenap;
int totalGenap=0;
double avg;

System.out.print("Masukkan angka: ");
bil = input.nextInt();
jmlBilGenap = bil/2;
System.out.println("Jumlah bilangan dari 1 sampai "+ bil + " adalah "+ jmlBilGenap);
System.out.print("Angka genap dalam range tersebut adalah ");

for(int i=2; i<=bil; i+=2){
    System.out.print(i);
    if(i!=bil){
        System.out.print(", ");
    }
    totalGenap += i;
}
    avg = totalGenap/jmlBilGenap;
    System.out.println("\nhasil penjumlahan angka genap 1 sampai " + bil + " adalah " + totalGenap);
    System.out.println("Rata-rata angka genap  dari 1 sampai " + bil + " adalah " + avg);
```

    Masukkan angka: 10
    Jumlah bilangan dari 1 sampai 10 adalah 5
    Angka genap dalam range tersebut adalah 2, 4, 6, 8, 10
    hasil penjumlahan angka genap 1 sampai 10 adalah 30
    Rata-rata angka genap  dari 1 sampai 10 adalah 6.0


2. Buatlah program untuk menampilkan angka 1 hingga angka masukan pengguna secara berurutan dan melompati angka kelipatan 5. Seperti tampilan di bawah ini
<p align="left">
<img width="184" height="328" src="images/tugas1.jpg" align="left">
</p>


```Java
// Ketik kode program disini
import java.util.Scanner;
Scanner input = new Scanner(System.in);
System.out.print("Masukkan angka: ");
int angka = input.nextInt();

for(int i=1; i<=angka; i++){
    if(i%5 == 0) continue;
    System.out.println(i);
}
```

    Masukkan angka: 19
    1
    2
    3
    4
    6
    7
    8
    9
    11
    12
    13
    14
    16
    17
    18
    19

3. Buatlah sebuah program yang menampilkan deret bilangan fibonacci sebagai berikut. Dimana bilangan yang terletak di sebelah kanan adalah hasil penjumlahan dari 2 bilangan sebelumnya
 <p align="left">
    <img width="451" height="226" src="images/fibo.png" align="left">
    </p>



```Java
// Ketik kode program disini
import java.util.Scanner;
Scanner input = new Scanner(System.in);
int jumlah;
int satu = 0;
int dua = 1;
System.out.print("Masukkan banyak bilangan fibonacci: ");
int bil = input.nextInt();

int i;
for(i=0; i<bil; ++i){
    System.out.print("Sum of: " + satu + " + " + dua + " = ");
    jumlah = satu + dua;
    satu = dua;
    dua = jumlah;
    System.out.println(jumlah);
}
```

    Masukkan banyak bilangan fibonacci: 6
    Sum of: 0 + 1 = 1
    Sum of: 1 + 1 = 2
    Sum of: 1 + 2 = 3
    Sum of: 2 + 3 = 5
    Sum of: 3 + 5 = 8
    Sum of: 5 + 8 = 13
```
