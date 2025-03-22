# TP4DPBO2025C1

Saya Nina Wulandari dengan NIM 2312091 mengerjakan Tugas Praktikum 4 dalam mata kuliah DPBO untuk keberkahan-Nya maka saya tidak melakukan kecurangan seperti yang telah dispesifikasikan. Aamiin

# Desain Class
![Diagram TP4 drawio](https://github.com/user-attachments/assets/10954807-0bde-4936-9260-8a0a082bae0e)

# Desain Form
![FORM](https://github.com/user-attachments/assets/622954bb-284f-40af-b70a-7cacad44da29)


# Penjelasan Atribut dan Methods
1. Class Mahasiswa (Model) → Kelas ini merepresentasikan objek mahasiswa.
   * string nim
   * string nama
   * string jenisKelamin
   * string statusMahasiswa

     Methods:
      * getter dan setter untuk mengakses dan memodifikasi atribut mahasiswa.
    
2. Class Menu (View + Controller) → Kelas ini adalah GUI yang mewarisi JFrame
   * int selectedIndex
   * ArrayList<Mahasiswa> listMahasiswa
   * JPanel mainPanel
   * JTextField nimField
   * JTextField namaField
   * JTable mahasiswaTable
   * JButton addUpdateButton
   * JButton cancelButton
   * JComboBox<String> jenisKelaminComboBox
   * JComboBox<String> statusMahasiswaComboBox
   * JButton deleteButton
   * JLabel titleLabel
   * JLabel nimLabel
   * JLabel namaLabel
   * JLabel jenisKelaminLabel
   * JLabel StatusMahasiswaLabel
     
     Methods:
        * setTable() → membuat tabel untuk menampilkan data mahasiswa dari listMahasiswa.
        * insertData() → Menambahkan data mahasiswa baru ke dalam listMahasiswa.
        * updateData() → Memperbarui data mahasiswa yang dipilih pada listMahasiswa.
        * deleteData() → Menghapus data mahasiswa dari listMahasiswa dan melakukan konfirmasi sebelum menghapus.
        * clearForm() → Mengosongkan form dan mengatur ulang tombol yaitu, "Update" menjadi "Add", invisible tombol "Delete", dan reset index.
        * populateList() → Mengisi listMahasiswa dengan contoh data mahasiswa.


# Penjelasan Alur Program
 * Program dimulai dengan Jendela GUI yang muncul setelah di run.
 * Jendela GUI akan menampilkan form dan daftar data mahasiswa.
 * Disini saya menambahkan 1 atribut dan formnya sebagai modifikasi tugas bonus, atribut tersebut adalah statusMahasiswa yang mana menunjukkan apakah mahasiswa tersebut aktif, sedang cuti, sudah         lulus, atau dropout. Untuk formnya sendiri saya gunakan JComboBox supaya bisa dropdown pilihannya.

Terdapat 3 fitur yang dapat dilakukan oleh user dengan alur berikut.
   1. Menambahkan Data
       * Untuk menambahkan data mahasiswa, user mengisi form dan memasukkan data mahasiswa (NIM, Nama, Jenis Kelamin, Status) kemudian klik button Add.
       * Objek Mahasiswa dibuat berdasarkan input kemudian objek ini dimasukkan ke dalam ArrayList<Mahasiswa>.
       * Muncul pop-up notifikasi sukses.
       * Nama dan status mahasiswa ditampilkan di JList.
       * Setelah menambahkan mahasiswa, input field dikosongkan agar bisa diisi lagi.
         
   2. Mengupdate Data
       * Untuk mengupdate data, user klik salah satu baris data mahasiswa di JList, lalu form yang semula kosong akan terisi dengan data tersebut.
       * Button Add akan berubah nama menjadi Update
       * Lakukan perubahan data yang diperlukan kemudian klik Update.
       * Muncul pop-up notifikasi sukses.
       * Nama dan status mahasiswa yang baru diupdate ditampilkan di JList.
       * Setelah menambahkan mahasiswa, input field dikosongkan agar bisa diisi lagi.
  
  3. Menghapus Data
       * Untuk menghapus data, user klik salah satu baris data mahasiswa di JList, lalu form yang semula kosong akan terisi dengan data tersebut.
       * Button Add akan berubah nama menjadi Update
       * Lalu klik button Delete.
       * Muncul pop-up confirmation prompt, untuk konfirmasi penghapusan data
       * Pilih Yes untuk menghapus data, pilih No untuk cancel
       * Nama dan status mahasiswa yang baru dihapus diremove dari tampilan di JList.
       * Setelah menambahkan mahasiswa, input field dikosongkan agar bisa diisi lagi.


# Dokumentasi Program
https://github.com/user-attachments/assets/ce80923a-e84d-45e4-8736-cb87ec218bc4


