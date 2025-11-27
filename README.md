## Tes flutter preview di browser

> [!NOTE]   
> Pada praktik ini digunakan Windows PowerShell untuk menjalankan beberapa perintah CLI Flutter.   


### Implementasi   

1. Buat project baru (**e.g.** `flutter create tes_preview`)     
   ```flutter
   flutter create <nama-project>
   ```
   <img src="img/1.png" width="500">

2. Masuk ke folder project (**e.g.** `cd tes_preview`)  
   ```bash
   cd <nama-project>
   ```
   <img src="img/2_1.png" width="500">  
   

3. Buka file main.dart di `<nama-project>\lib\main.dart`  

   <img src="img/2.png" width="500">


4. **Pada file `main.dart`, tambahkan import witget_previews**
   ```flutter
   import 'package:flutter/widget_previews.dart';
   ```  
   <img src="img/3.png" width="500">

5. **pada bagian akhir code, tambahakan** 
   ```flutter
   @Preview(name: 'My Sample Text')
   Widget mySampleText() {
     return const Text('Hello, World!');
   }
   ```   
   <img src="img/4.png" width="500">  
   
   > Simpan perubahan file main.dart  

6. _**Jalankan flutter doctor**_    
   ```flutter
   fluuter doctor
   ``` 
   <img src="img/5.png" width="500"> 

7. _**Jalankan flutter pub get**_
   ```flutter
   flutter pub get  
   ```
   <img src="img/6.png" width="500">   

   > Kalau ingin memperbarui ke versi terbaru dari semua dependency:
   > `flutter pub upgrade`   

8. **Jalankan preview**
    ```flutter
    flutter widget-preview start
    ```   
    <img src="img/7.png" width="500">   
   
   Tampilan di browser (dalam praktik ini menggunakan chrome browser)  
   <img src="img/8.png" width="500">

9. Lakukan modifikasi, contoh:
   ```
   Text('HALO');
   ```   
   <img src="img/8.png" width="500">
   
   Kemudian simpan (`Ctrl+S`)  dan lihat perubahan   
   <img src="img/8_2.png" width="500">
   
   update otomatis dilakukan saat perubahan disimpan.

10. Menampilkan app  
    
    Ubah `Text('HALO');` jadi:
    ```
    MyApp();
    ```   
     Save dan lihat perubahan.   
    <img src="img/9.png" width="500">  

   

 11. Hentikan running preview:   
     `Ctrl`+`C` kemudian `y` lalu tekan `Enter`   
     <img src="img/10.png" width="500">  

