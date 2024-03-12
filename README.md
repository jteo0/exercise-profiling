# Modul 5
1. JMeter menggunakan thread group dan meng-approach performance testing dengan menggunakan thread profiling. Intellij Profiler menggunakan CPU dan Memory profiling, dengan bagian yang mengambil waktu/memori yang paling tinggi bisa dilihat dari hasil profiling. JMeter hanya menunjukkan hasil jalan thread secara langsung (bukan bagiannya).

2. Proses profiling menolong saya untuk melihat apakah program berjalan secara konsisten, serta kecepatan jalannya secara spesifik. Bagian yang paling pelan atau yang sebaiknya dioptimisasi jelas terlihat jika menggunakan Intellij Profiler.

3. Iya. Intellij Profilier menolong saya melihat bagian dari program saya yang masih jelas bisa dioptimisasi lagi, atau yang <i>slowing down</i> seluruh program.

4. Kesulitan terbesar yang saya hadapi dalam profiling dan performance testing pada modul ini adalah dalam mengkomparasi performance pre dan post refactoring dari /highest-gpa. Kedua method yang saya ubah sebelumnya memiliki perubahan performance yang cukup jelas, sedangkan saat saya mengecek kecepatan run endpoint menggunakan postman, performance post-refactoring kurang konsisten, dan juga tidak begitu beda dengan yang pre-refactoring. Kesulitan ini diselesaikan dengan menggunakan fitur di Intellij Profiler yang menunjukkan runtime suatu method saat dilakukan profiling.

5. Menurut saya, keunggulan utamanya adalah saya dapat melihat secara jelas runtime setiap bagian (sampai method), sehingga bisa melihat kelemahan/weak point dimana program saya berjalan dengan relatif pelan.

6. Yang pertama saya akan lakukan adalah run proses profiling dengan keduanya lagi. Jika setelah itu masih berbeda/tidak konsisten sama, saya akan mengecek ulang program saya/program lain yang sedang berjalan di sistem saya yang mungkin dapat mempengaruhi proses performance testing.

7. Saya mengimplementasi strategi mengecek hasil dari suatu endpoint dengan menggunakan Postman sebelum melakukan perubahan apapun. Setelah itu, saya mencari nagian program yang terlihat bisa dioptimisasi lagi, dan saya coba untuk refactor dan membuatnya lebih optimized. Setelah diubah, saya menjalankannya dan cek hasil endpointnya dari postman lagi untuk mengecek bahwa hasilnya masih sama dan ada perubahan runtime positif (lebih cepat) yang signifikan. Saya mengecek postman beberapa kali untuk memastikan bahwa hasilnya konsisten.


Screenshots:

JMeter /all-student-name sebelum refactor + hasil commandline
<img src="Screenshots/all-student-name jmeter 1.png">
<img src="Screenshots/all-student-name jmeter 2.png">
<img src="Screenshots/all-student-name jmeter 3.png">
<img src="Screenshots/all-student-name jmeter 4.png">
<img src="Screenshots/all-student-name command-line.png">

JMeter /highest-gpa sebelum refactor + hasil commandline
<img src="Screenshots/highest-gpa jmeter 1.png">
<img src="Screenshots/highest-gpa jmeter 2.png">
<img src="Screenshots/highest-gpa jmeter 3.png">
<img src="Screenshots/highest-gpa jmeter 4.png">
<img src="Screenshots/highest-gpa command-line.png">

Optimize /all-student-name
Pre-refactoring
<img src="Screenshots/all-student-name pre-refactor.png">

Post-refactoring
<img src="Screenshots/all-student-name post-refactor.png">

Optimize /highest-gpa
Pre-refactoring
<img src="Screenshots/highest-gpa pre-refactor.png">

Post-refactoring
<img src="Screenshots/highest-gpa post-refactor.png">

JMeter /all-student-name setelah refactor
<img src="Screenshots/all-student-name post-jmeter 1.png">
<img src="Screenshots/all-student-name post-jmeter 2.png">
<img src="Screenshots/all-student-name post-jmeter 3.png">
<img src="Screenshots/all-student-name post-jmeter 4.png">

JMeter /highest-gpa setelah refactor
<img src="Screenshots/highest-gpa post-jmeter 1.png">
<img src="Screenshots/highest-gpa post-jmeter 2.png">
<img src="Screenshots/highest-gpa post-jmeter 3.png">
<img src="Screenshots/highest-gpa post-jmeter 4.png">
