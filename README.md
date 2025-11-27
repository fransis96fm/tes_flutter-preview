### Tes flutter preview

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

