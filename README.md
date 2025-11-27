### Tes flutter preview di browser

> [!NOTE]   
> Disini saya menggunakan windows powershell untuk menjalankan beberapa cli flutter

1. Buat project baru (**e.g.** `flutter create tes_preview`)     
   ```flutter
   flutter create <nama-project>
   ```


2. Masuk ke folder project (**e.g.** `cd tes_preview`)  
   ```bash
   cd <nama-project>
   ```  

3. Buka file main.dart di `<nama-project>\lib\main.dart`  

4. Pada file `main.dart`, tambahkan import witget_previews
   ```flutter
   import 'package:flutter/widget_previews.dart';
   ```   

5. pada bagian akhir code, tambahakan 
   ```flutter
   @Preview(name: 'My Sample Text')
   Widget mySampleText() {
     return const Text('Hello, World!');
   }
   ```
   > Simpan perubahan file main.dart 

6. Jalankan flutter doctor  
   ```flutter
   fluuter doctor
   ```

7. Jalankan flutter pub get
   ```flutter
   flutter pub get  
   ```

   > Kalau ingin memperbarui ke versi terbaru dari semua dependency:
   > `flutter pub upgrade`   

8. Jalankan preview
   ```flutter
   flutter widget-preview start
   ```

9. Tampilan di browser (dalam praktik ini menggunakan chrome browser)  


10. Lakukan modifikasi, contoh:
   ```
   Text('HALO');
   ```
   Kemudian simpan (`Ctrl+S`)  dan lihat perubahan
    <img>

    update otomatis dilakukan saat perubahan disimpan.

11. Menampilkan app  
    
    Ubah `Text('HALO');` jadi:
    ```
    MyApp();
    ```

    Save dan lihat perubahan.

 12. Hentikan running preview:

    `Ctrl`+`C` kemudian `y` lalu tekan `Enter`
    <img>
