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
   
   <a href="">
      <img src="img/2.png" width="500">
   </a>    

<p align="center">
  <a href="img/2.png">
    <img src="img/2.png" alt="Demo zoom" style="max-width: 100%; height: auto; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);" />
  </a>
</p>


5. Pada file `main.dart`, tambahkan import witget_previews
   ```flutter
   import 'package:flutter/widget_previews.dart';
   ```  
   <img src="img/3.png" width="500">

6. pada bagian akhir code, tambahakan 
   ```flutter
   @Preview(name: 'My Sample Text')
   Widget mySampleText() {
     return const Text('Hello, World!');
   }
   ```   
   <img src="img/4.png" width="500">  
   
   > Simpan perubahan file main.dart  

7. Jalankan flutter doctor    
   ```flutter
   fluuter doctor
   ``` 
   <img src="img/5.png" width="500"> 

8. Jalankan flutter pub get
   ```flutter
   flutter pub get  
   ```
   <img src="img/6.png" width="500">   

   > Kalau ingin memperbarui ke versi terbaru dari semua dependency:
   > `flutter pub upgrade`   

9. Jalankan preview
   ```flutter
   flutter widget-preview start
   ```   
   <img src="img/7.png" width="500">   
   
   Tampilan di browser (dalam praktik ini menggunakan chrome browser)  
   <img src="img/8.png" width="500">

11. Lakukan modifikasi, contoh:
   ```
   Text('HALO');
   ```
   Kemudian simpan (`Ctrl+S`)  dan lihat perubahan
    <img>

    update otomatis dilakukan saat perubahan disimpan.

12. Menampilkan app  
    
    Ubah `Text('HALO');` jadi:
    ```
    MyApp();
    ```

    Save dan lihat perubahan.

 12. Hentikan running preview:

    `Ctrl`+`C` kemudian `y` lalu tekan `Enter`
    <img>


<script src="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.11.4/js/lightbox.min.js"></script>
<link href="https://cdnjs.cloudflare.com/ajax/libs/lightbox2/2.11.4/css/lightbox.min.css" rel="stylesheet" />
