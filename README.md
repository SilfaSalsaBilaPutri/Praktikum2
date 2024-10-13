Buatlah kode program java untuk:
- Mendeklarasikan class Person, dengan atribut Nama, JenisKelamin, Umur dan lengkapi dengan access modifier.
- Buatlah dua buah objek dari class Person bernama Anton dan Riko dan panggil method setter dan getter.
![Screenshot 2024-10-13 212053](https://github.com/user-attachments/assets/60e59072-a986-4428-952d-567cd3368c2f)

- Mendeklarasikan class person
```
    public class Person {
    // Deklarasi atribut
    private String nama;
    private String jenisKelamin;
    private int umur;

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
