# Praktikum 7 - Pemrograman Web
```
Veno Setyoaji Wiratama
311910363
TI.19.A.2
Universitas Pelita Bangsa
```
## Buka XAMPP dan jalankan `Apache`
![XAMPP](https://user-images.githubusercontent.com/22215113/117587513-87db7400-b148-11eb-80d4-48c837299b82.png)

## Buat Folder `lab7_php_dasar` pada root directory web server (C:\xampp\htdocs) dan Buat file baru dengan nama `php_dasar.php` pada directory tersebut.
![FOLDER XAMPP](https://user-images.githubusercontent.com/22215113/117587545-accfe700-b148-11eb-803f-6ccfa8402424.png)
![FOLDER XAMPP 2](https://user-images.githubusercontent.com/22215113/117587561-c5400180-b148-11eb-8fd0-0f4983d5c364.png)

## Untuk mengakses direktory tersebut pada web server dengan mengakses URL: http://localhost/lab7_php_dasar/
![LANGKAH 2 MEMBUAT FILE PHP 2](https://user-images.githubusercontent.com/22215113/117587668-48f9ee00-b149-11eb-9b03-a8ce568dad5c.png)

## LANGKAH 1
### Coding dasar pengenalan PHP
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>
<body>
    <h1>Belajar PHP Dasar</h1>
        <?php
            echo "Hello World";
        ?>
</body>
</html>
```
![LANGKAH 2 MEMBUAT FILE PHP](https://user-images.githubusercontent.com/22215113/117587678-4d260b80-b149-11eb-92b1-d326106eeca0.png)

## LANGKAH 2
### Menambahkan Variable pada Program
```
<h2>Menggunakan Variable</h2>
<?php
    $nim = "0411500400";
    $nama = 'Abdullah';
    echo "NIM : " . $nim . "<br>";
    echo "Nama : $nama";
?>
```
![LANGKAH 3 menggunakan variable](https://user-images.githubusercontent.com/22215113/117587733-83fc2180-b149-11eb-9017-1cdbf122170b.png)

## LANGKAH 3
### Predefine Variable $_GET. Untuk mengaksesnya gunakan URL:http://localhost/lab7_php_dasar/php_dasar.php?nama=VenoSW
```
<h2>Predefine Variable</h2>
<?php
    echo 'Selamat Datang ' . $_GET['nama'];
?>
```
![LANGKAH 4 predefine variable](https://user-images.githubusercontent.com/22215113/117587808-e5bc8b80-b149-11eb-84b8-0822df1a2251.png)

## LANGKAH 4
### Membuat Form Input
```
<h2>Form Input</h2>
<form method="post">
    <label>Nama: </label>
    <input type="text" name="nama">
    <input type="submit" value="Kirim">
</form>
<?php
    echo 'Selamat Datang ' . $_POST['nama'];
?>
```
![LANGKAH 5 form input](https://user-images.githubusercontent.com/22215113/117587870-37651600-b14a-11eb-8450-410ffec667fd.png)

## LANGKAH 5
### Operator
```
<h2>Operator</h2>
<?php
    $gaji = 1000000;
    $pajak = 0.1;
    $thp = $gaji - ($gaji*$pajak);
    echo "Gaji sebelum pajak = Rp. $gaji <br>";
    echo "Gaji yang dibawa pulang = Rp. $thp";
?>
```
![LANGKAH 6 operator](https://user-images.githubusercontent.com/22215113/117587929-9a56ad00-b14a-11eb-93bd-5fbee1e3717b.png)

## LANGKAH 6
### Kondisi IF
```
<h2>Kondisi IF</h2>
    <?php
        $nama_hari = date("l");
        if ($nama_hari == "Sunday") {
        echo "Minggu";
        } elseif ($nama_hari == "Monday") {
        echo "Senin";
        } else {
        echo "Selasa";
        }
    ?>
```
![LANGKAH 7 kondisi if](https://user-images.githubusercontent.com/22215113/117587954-bd815c80-b14a-11eb-8eaf-36a8cb5b9630.png)

## LANGKAH 7
### Kondisi SWITCH
```
<h2>Kondisi SWITCH</h2>
    <?php
    $nama_hari = date("1");
    switch ($nama_hari) {
        case "Sunday":
            echo "Minggu";
            break;
        case "Monday":
            echo "Senin";
            break;
        case "Tuesday":
            echo "Selasa";
            break;
        default:
            echo "Sabtu";
        }
    ?>
```
![LANGKAH 8 kondisi switch](https://user-images.githubusercontent.com/22215113/117587970-d5f17700-b14a-11eb-9157-caf430539c49.png)

## LANGKAH 8
### Perulangan FOR
```
<h2>Perulangan FOR</h2>
   <?php
        echo "Perulangan 1 sampai 10 <br />";
        for ($i=1; $i<=10; $i++) {
            echo "Perulangan ke: " . $i . '<br />';
        }

        echo "Perulangan Menurun dari 10 ke 1 <br />";
        for ($i=10; $i>=1; $i--) {
            echo "Perulangan ke: " . $i . '<br />';
        }
   ?>
```
![LANGKAH 9 perulangan FOR](https://user-images.githubusercontent.com/22215113/117587989-ebff3780-b14a-11eb-8090-a5c75be6dcc8.png)

## LANGKAH 9
### Perulangan WHILE
```
<h2>Perulangan WHILE</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
        $i=1;
        while ($i<=10) {
            echo "Perulangan ke: " . $i . '<br />';
            $i++;
        }
    ?>
```
![LANGKAH 10 perulangan WHILE](https://user-images.githubusercontent.com/22215113/117588009-02a58e80-b14b-11eb-993f-d3cd5ca89edb.png)

## LANGKAH 10
### Perulangan DOWHILE
```
<h2>Perulangan DOWHILE</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
        $i=1;
        do {
            echo "Perulangan ke: " . $i . '<br />';
            $i++;
        } while ($i<=10);
    ?>
```
![LANGKAH 11 perulangan DOWHILE](https://user-images.githubusercontent.com/22215113/117588027-1b15a900-b14b-11eb-8b41-b267aad11917.png)

## TUGAS
### Buatlah program PHP sederhana dengan menggunakan form input yang menampilkan nama, tanggal lahir dan pekerjaan. Kemudian tampilkan outputnya dengan menghitung umur berdasarkan inputan tanggal lahir. Dan pilihan pekerjaan dengan gaji yang berbeda-beda sesuai pilihan pekerjaan.

* CODING
```
    <h2>TUGAS</h2>
    <form method="post">
            <label>Nama: </label>
            <input type="text" name="nama">
            <br>
            <label>Tanggal Lahir: </label>
            <input type="text" name="tgl_lahir">
            <br>
            <label>Pekerjaan: 
            <select name='pekerjaan'>
                <option value='Direktur'>Direktur</option>
                <option value='Manager'>Manager</option>
                <option value='Staff'>Staff</option>
                <option value='Operator'>Operator</option>
            </select>
            </label>
            <br>
            <input type="submit" value="Kirim">
    </form>
    <?php
        # Memanggil Nama
        echo 'Nama: ' . $_POST['nama'];

        # Merubah Tanggal Lahir menjadi Umur (Tahun)
        $tgl_lahir = @$_POST['tgl_lahir'];

        $lahir = new DateTime($tgl_lahir);
        $hari_ini = new DateTime();

        $diff = $hari_ini->diff($lahir);

        # Memanggil fungsi umur yg sudah dibuat diatas
        echo "<br> Umur: ". $diff->y ." Tahun";

        # Memanggil pekerjaan
        echo "<br> Pekerjaan: ". $_POST['pekerjaan'];

        # Kondisi if pekerjaan untuk menentukan gaji
        $pekerjaan = @$_POST['pekerjaan'];

        if($pekerjaan == "Direktur"){
            echo '<br> Gaji: Rp. 10.000.000,-';
        }elseif($pekerjaan == "Manager"){
            echo '<br> Gaji: Rp. 7.000.000,-';
        }elseif($pekerjaan == "Staff"){
            echo '<br> Gaji: Rp. 5.000.000,-';
        }elseif($pekerjaan == "Operator"){
            echo '<br> Gaji: Rp. 4.000.000,-';
        }
    ?>
```
![TUGAS (CODING)](https://user-images.githubusercontent.com/22215113/117588056-4d270b00-b14b-11eb-8721-a3ce36bf2deb.png)
![TUGAS (CODING) 2](https://user-images.githubusercontent.com/22215113/117588118-a1ca8600-b14b-11eb-87a3-43e6803a1b4f.png)
```
Perbedaan metode POST dan GET
* Metode GET akan menampilkan semua data dalam url (yang kemudian disebut sebagai query string).
* Sedangkan POST akan menyimpan data di dalam body request tanpa menampilkannya secara langsung di dalam URL.
```
* OUTPUT
![TUGAS (OUTPUT)](https://user-images.githubusercontent.com/22215113/117588198-25847280-b14c-11eb-9cc2-974c5906117f.png)
