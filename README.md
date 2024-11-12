# Tugas 8 PrakPemMob

## Penjelasan

### 1. Tampilan Awal

<img src="src/assets/image/1.png">

<p> Pada mahasiswa.page.ts digunakan metode getMahasiswa() untuk mengambil data dari API melalui ApiService. Metode ini dipanggil saat komponen diinisialisasi melalui ngOnInit(), kemudian data yang diterima disimpan dalam variabel dataMahasiswa. Potongan kode berikut menunjukkan pemanggilan API dan penyimpanan data: <p>

```typescript
ngOnInit() {
  this.getMahasiswa();
}

getMahasiswa() {
  this.api.tampil('tampil.php').subscribe({
    next: (res: any) => {
      console.log('sukses', res);
      this.dataMahasiswa = res;
    },
    error: (err: any) => {
      console.log(err);
    },
  });
}

### 2. Menambahkan Data Baru

<img src="src/assets/image/2.png">

### 3. Menampilkan Data Setelah Ditambahkan

<img src="src/assets/image/3.png">

### 4. Edit Data

<img src="src/assets/image/4.png">

### 5. Menampilkan Data Setelah Diedit

<img src="src/assets/image/5.png">

### 6. Menghapus Data

<img src="src/assets/image/6.png">

### 7. Menampilkan Data Setelah Dihapus

<img src="src/assets/image/7.png">


### Demo Aplikasi

<img src="src/assets/image/Demo.gif">