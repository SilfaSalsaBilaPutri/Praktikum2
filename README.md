Buatlah kode program java untuk:
- Mendeklarasikan class Person, dengan atribut Nama, JenisKelamin, Umur dan lengkapi dengan access modifier.
- Buatlah dua buah objek dari class Person bernama Anton dan Riko dan panggil method setter dan getter.
![Screenshot 2024-10-13 212053](https://github.com/user-attachments/assets/60e59072-a986-4428-952d-567cd3368c2f)
# Pengimplenmentasiannya
- Mendeklarasikan class person
```
    public class Person {
    // Deklarasi atribut
    private String nama;
    private String jenisKelamin;
    private int umur;
```
Code di atas menggunakan access modifier private artinya atribut ini hanya dapat diakses dari dalam kelas Person itu sendiri. Kelas atau objek lain tidak dapat langsung mengakses atribut ini, sehingga melindungi data tersebut dari manipulasi langsung dari luar kelas.

```
    // Constructor untuk menginisialisasi atribut
    public Person(String nama, String jenisKelamin, int umur) {
        this.nama = nama;
        this.jenisKelamin = jenisKelamin;
        this.umur = umur;
    }

    // Getter dan Setter untuk atribut nama
    public String getNama() {
        return nama;
    }

    public void setNama(String nama) {
        this.nama = nama;
    }

    // Getter dan Setter untuk atribut jenisKelamin
    public String getJenisKelamin() {
        return jenisKelamin;
    }

    public void setJenisKelamin(String jenisKelamin) {
        this.jenisKelamin = jenisKelamin;
    }

    // Getter dan Setter untuk atribut umur
    public int getUmur() {
        return umur;
    }

    public void setUmur(int umur) {
        this.umur = umur;
    }

    // Method untuk menampilkan informasi tentang person
    public void tampilkanInfo() {
        System.out.println("Nama: " + nama);
        System.out.println("Jenis Kelamin: " + jenisKelamin);
        System.out.println("Umur: " + umur);
    }
 ```
Code di atas menggunakan access modifier public untuk mengakses atau mengubah nilai atribut private diperlukan metode getter dan setter yang bersifat public. Pada metode ini memungkinkan siapa pun yang memiliki objek Person untuk mengakses atau mengubah nilai atribut tersebut secara aman, tanpa mengaksesnya langsung. Pada metode tampilkanInformasi bisa diakses dari luar kelas untuk menampilkan informasi mengenai objek Person secara lengkap, metode tampilkanInformasi juga bisa diakses oleh kode lain.
-  Membuat dua buah objek dari class Person dan memanggil method setter dan getter
```
    // Main method untuk menjalankan program
    public static void main(String[] args) {
        // Membuat objek Person bernama Antor dan Riko
        Person antor = new Person("Antor", "Laki-laki", 18);
        var riko = new Person("Riko", "Laki-laki", 19);

        // Menampilkan informasi untuk Antor
        System.out.println("Informasi Antor:");
        antor.tampilkanInfo();

        // Menampilkan informasi untuk Riko
        System.out.println("\nInformasi Riko:");
        riko.tampilkanInfo();
    }
```
# Hasil output
![image](https://github.com/user-attachments/assets/edf5ffd3-ead8-459b-9719-ca8453d089f4)
