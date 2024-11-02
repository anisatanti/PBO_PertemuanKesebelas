# **Tugas PBO TM 11 (Upload File CSV kedalam Aplikasi GUI Netbeans)**
___
## **Daftar Isi**

- [Koneksi](https://github.com/anisatanti/PBO_PertemuanKesebelas/blob/main/DbUtils.java)
- [FrameMataKuliah.Form](https://github.com/anisatanti/PBO_PertemuanKesebelas/blob/main/FrameMataKuliah.form)
- [FrameMataKuliah.Java](https://github.com/anisatanti/PBO_PertemuanKesebelas/blob/main/FrameMataKuliah.java)
- [reportmatakuliah.jasper](https://github.com/anisatanti/PBO_PertemuanKesebelas/blob/main/reportmatakuliah.jasper)
- [reportmatakuliah.jrxml](https://github.com/anisatanti/PBO_PertemuanKesebelas/blob/main/reportmatakuliah.jrxml)
___
## **_Deskripsi_**

Proyek ini merupakan Tugas Pertemuan Kesebelas Mata Kuliah Pemrograman Berorientasi Objek. Membuat Aplikasi CRUD pada Netbeans Java yang terhubung dengan Aplikasi basis data PostgreSQL yang ditambah dengan button Upload. Upload yang dimaksud adalah menginput data pada file CSV (Comma Separated Value) yang telah dibuat pada Microsoft Excel kemudian ditampilkan pada Aplikasi GUI Data Mata Kuliah. File CSV merupakan format file yang digunakan untuk menyimpan data dalam bentuk tabel sederhana, setiap baris mewakili satu entri atau record, dan setiap kolom dipisahkan dengan tanda koma (,) atau titik koma (;). File CSV dirancang untuk menjadi cara mudah mengekspor data dan mengimpornya ke program lain.

___
## **Langkah-langkah Upload Data Menggunakan Format File CSV Pada GUI Netbeans:**
1.	Membuat data Mata Kuliah  dengan 4 kolom yang berisi Kode Mata Kuliah, SKS, Nama Mata Kuliah, dan Semester Ajar.
   
     ![image](https://github.com/user-attachments/assets/53945bb5-282c-4170-bb6b-80d49ec9a863)

2.	Menyimpan data Mata Kuliah dalam bentuk CSV (Comma Separated Values)
   
     ![image](https://github.com/user-attachments/assets/c1a8e6ea-01dc-40d6-b7c1-317f3d8d0e73)

3.	Membuat database baru pada Aplikasi PostgreSQL dengan cara klik kanan icon database kemudian klik create, klik database.
   
     ![image](https://github.com/user-attachments/assets/c70b6f9b-86c6-4170-a0f0-f514311e73c7)

4.	Beri nama database “Mata_Kuliah”.
   
     ![image](https://github.com/user-attachments/assets/6fc718fe-ea6c-4406-a203-4e2a0994fc60)

5.	Membuat tabel MataKuliah beserta atributnya.

     ![image](https://github.com/user-attachments/assets/f4566cc6-9a71-4cb1-81fd-8162737f67b0)

6.	Membuat project baru pada Netbeans dengan cara klik New Project, pada categories pilih Java with Ant, pada Projects pilih Java Aplication kemudian klik Next.

     ![image](https://github.com/user-attachments/assets/47720566-ea91-425d-8b28-7d5bbb5b5d63)

7.	Beri nama project baru dengan nama PBO_PertemuanKesebelas, unchecklist pada Create Main Class kemudian klik Finish.

     ![image](https://github.com/user-attachments/assets/117d5262-3487-46b4-9745-edbc096fee8e)

8.	Membuat Kelas koneksi “DbUtils”  dengan cara klik kanan pada package report, klik New, klik Java Class. Isi code kelas DbUtils.

     ![image](https://github.com/user-attachments/assets/62291071-104f-4983-9d7f-6e839c2273dd)

9.	Menambahkan button Upload pada desain GUI Mata Kuliah. Tampilan GUI Mata Kuliah Berisi Kode MK, SKS, Nama MK, dan Semester Ajar yang diinput menggunakan JTextField, button Insert, Update, Delete, Clear, Cetak, Upload, dan Exit menggunakan JButton, serta tabel Mata Kuliah menggunakan JTable.

     ![image](https://github.com/user-attachments/assets/fe167ecc-c0f8-4c71-b48f-45ac3b09dac2)

10.	Menambahkan Library PostgreSQL dengan cara klik kanan pada Library project kemudian klik Add Library.

     ![image](https://github.com/user-attachments/assets/2087e90b-c067-4747-b7c9-8d2ad393ed6c)

11.	Setelah muncul pop up, pilih PostgreSQl JDBC Driver kemudian klik Add Library.

     ![image](https://github.com/user-attachments/assets/ba89ed86-04c8-45c1-a87b-fd0d0bb52445)

12.	Menambahkan Library Jasperreport dengan cara klik kanan pada Libraries, klik Add Jar/Folder.

     ![image](https://github.com/user-attachments/assets/21e76d58-c4df-476c-894f-1c053307ec50)

    File library jasperreport berhasil ditambahkan.

     ![image](https://github.com/user-attachments/assets/8364256e-2f05-4d16-badc-2e21124809a5)

13.	Berikut beberapa import yang digunakan pada program GUI Data Mata Kuliah.

     ![image](https://github.com/user-attachments/assets/135568b1-4f9e-481a-ad22-d3f115271a83)

14.	Berikut code untuk koneksi program dengan database postgresql disertai method koneksi.

     ![image](https://github.com/user-attachments/assets/9e2352a9-2604-4cb1-8404-4eec33503323)

15.	Membuat method tampil untuk menampilkan semua data pada JTable. Method peringatan, Kemudian method clear untuk menghapus text pada JTextField.

     ![image](https://github.com/user-attachments/assets/56c99bbb-fdf4-4235-8ae2-19bf0486ec5c)

16. Berikut code btnInsert untuk menginput data ke dalam database yang akan ditampilkan pada tampilan GUI Data Mata Kuliah

     ![image](https://github.com/user-attachments/assets/731f08e2-7235-43e8-8ec1-c1749ed012cd)
     ![image](https://github.com/user-attachments/assets/a5374499-cdc2-4d32-b37b-f7dfc9df65bb)

17.	Berikut code btnUpdate untuk mengupdate data yang telah di inputkan.

     ![image](https://github.com/user-attachments/assets/6b2c46dd-0871-4ef1-942f-b5bed2486bc5)
   	 ![image](https://github.com/user-attachments/assets/ae86cd5e-2462-4f14-8dd8-01bba608773d)

18.	Berikut code btnDelete untuk menghapus data yang telah tersedia pada database.

     ![image](https://github.com/user-attachments/assets/bd19a9d1-cf5e-4637-95f0-922d44f9b31f)

19.	Berikut code btnClear, tblMK agar saat klik data pada tabel, data dapat tertampilkan pada JTextField, serta code btnExit untuk menutup tampilan GUI.

     ![image](https://github.com/user-attachments/assets/ada7aef2-8155-411c-aa58-1581c9fc6df5)

20.	Berikut code btnCetak untuk mencetak report yang akan dibuat.

     ![image](https://github.com/user-attachments/assets/0d70a577-65bc-4461-906d-dc550b0a52df)

21.	Membuat Desain jasperreport.
    
     ![image](https://github.com/user-attachments/assets/e48e1950-dff2-473c-8a88-8e56963b9dad)

22.	Mengisi code pada button Upload

     ![image](https://github.com/user-attachments/assets/6f23ebf5-821d-49f5-82f4-aae4a5777610)
   	 ![image](https://github.com/user-attachments/assets/1cb587e4-4a8f-4eb3-903b-9ffed93fcfdb)

23.	Eksekusi button Upload dengan cara klik button Upload lalu pilih file csv Data_Matkul yang telah dibuat kemudian klik Open.

     ![image](https://github.com/user-attachments/assets/7f4cab7e-a307-42f4-8258-a104966cd826)

24.	Klik ok untuk menampilkan data.

     ![image](https://github.com/user-attachments/assets/1cc21d8e-96fc-49f7-9e86-af96867b918b)

25.	Seluruh data pada file csv Data_Matkul berhasil ditampilkan.

     ![image](https://github.com/user-attachments/assets/52e5d84f-287f-40c2-9cb9-18c523204bf2)











    






















