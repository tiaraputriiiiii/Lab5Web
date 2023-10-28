# Lab5Web

```
Nama : Tiara Putri
NIM  : 312210009
Kelas : TI.22.A1
```

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Instruksi Praktikum|[Click Here](#instruksi-praktikum)|
|2|Langkah-langkah Praktikum|[Click Here](#langkah-langkah-praktikum)|
|3|Pertanyaan dan Tugas|[Click Here](#pertanyaan-dan-tugas)|

## Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama Lab5Web
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org


## Langkah-langkah Praktikum
> - Persiapan membuat dokumen HTML dengan nama file `lab5_javascript.html` seperti berikut :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
<script>
    document.write("Hello World");
    console.log("Hello World");
</script>
</body>
</html>
```

![1](https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/15b97103-8061-42e6-9f09-f1b8f3d516a0)

**1. Javascript Dasar**
> - Pemakaian `Alert` sebagai property window
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>alert box</title>
</head>
<body>
    <script language = "javascript" >
    <!-- 
    window.alert("ini merupakan pesan untuk anda");
    //-->
    </script>
</body>
</html>
```

![Alert](https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/42496716-c283-4031-b876-40952aa96f57)

> - Pemakaian `Method` dalam objek
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>skrip javascript</title>
</head>
<body>
percobaan memakai javascript:<br>
    <script language = "javascript" >
    <!-- 
    document.write("selamat mencoba javascript<br>");
    document.write("semoga sukses!");
    //-->
    </script>
</body>
</html>
```

![Method](https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/15a4b72f-d3a2-48e3-b42a-14115c3633a9)

> - Pemakaian `Prompt`
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>pemasukan data</title>
</head>
<body>
    <script language = "javascript" >
    <!-- 
    var nama = prompt("siapa nama anda?","masukkan nama anda");
    document.write("hai, " + nama);
    //-->
    </script>
</body>
</html>
```


https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/a8e86b7b-a46e-42d3-890b-fd6eec71b40b


> - Pembuatan `Fungsi` dan cara pemanggilannya
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
    function pesan(){
        alert ("memanggil javascript lewat body onload")
    }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
```

![fungsi](https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/4e475c46-98c5-4ec9-8fdd-bbdfedd4a911)

**2. Dasar Pemrograman di Javascript**
> - Operasi dasar `aritmatika`
```
<html>
<head>
    <title>contoh program javascript</title>

    <script language="javascript">
    function test (val1,val2)
    {
        document.write("<br>"+"perkalian : val1*val2 "+"<br>")
        document.write(val1*val2)
        document.write("<br>"+"pembagian : val1/val2 "+"<br>")
        document.write(val1/val2)
        document.write("<br>"+"penjumlahan : val1+val2 "+"<br>")
        document.write(val1+val2)
        document.write("<br>"+"pengurangan : val1-val2 "+"<br>")
        document.write(val1-val2)
        document.write("<br>"+"modulus : val1%val2 "+"<br>")
        document.write(val1%val2)
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
    </body>
    </html>
```



https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/630404cd-8229-41a7-bca9-b38fb9aaa6c2


> - Seleksi kondisi `(if..else)`
```
<html>
<head>
    <title>contoh if-else</title>
</head>
<body>
    <script language = "javascript">
    <!--
      var nilai = prompt("nilai (0-100): ", 0);
      var hasil = "";
      if (nilai >= 60)
      hasil = "lulus";
      else 
      hasil = "tidak lulus";
      document.write("hasil:" + hasil);   
    //-->
    </script>
</body>
</html>
```



https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/8f85a213-681e-4e05-acd0-c4668fce7699


> - Penggunaan operator `switch` untuk seleksi kondisi
```
<html>
<head>
    <title>contoh program javascript</title>

<script language="javascript">
function test ()
{
    val1=window.prompt("input nilai (1-5):")
    switch (val1)
    {
        case "1" :
            document.write("bilangan satu")
            break
        case "2" :
            document.write("bilangan dua")
            break
        case "3" :
            document.write("bilangan tiga")
            break
        case "4" :
            document.write("bilangan empat")
            break
        case "5" :
            document.write("bilangan lima")
            break
        default :
            document.write("bilangan lainnya")
    }
}
</script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
```


https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/133cc741-6aa3-4034-b96f-bc3de2d5d2a7


**3. Pembuatan Form**
> - Form `Input`
```
<html>
<head>
    <script language="javascript">
    function test () {
        var val1=document.kirim.T1.value
        if (val1%2==0)
            document.kirim.T2.value="bilangan genap"
        else
            document.kirim.T2.value="bilangan ganjil"
    }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20">
        MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
    </form>
</body>
</html>
```



https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/a9cb4583-a3a2-47bf-8462-c53269934ad8



> - Form `Button`
```
<html>
<head>
    <title>objek document</title>
</head>
<body>
    <script language = "javascript">
    <!--
    function ubahWarnaLB(warna) {
        document.bgColor = warna;
    }    
    function ubahWarnaLD(warna) {
        document.fgColor = warna;
    }
    //-->
    </script>

    <h1>tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLLOW')">
        <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
    </form>
    <script language = "javascript">
    <!--
    document.write("Dimodifikasi terakhir pada " +
    document.lastModified);
    //-->
    </script>
</body>
</html>
```



https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/c11cc236-e81d-4acb-982b-99fbd0db1037



**4. HTML DOM**
> - Pilihan menggunakan `checkbox` dengan perhitungan otomatis
```
<!--
File: daftar_menu.html
-->
<html>
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total) : 0);
            var harga = 0;

            if (ele.checked) {
                harga = ele.value
                total += parseInt(harga);
            } else {
                harga = ele.value;
                if (total > 0)
                    total -= parseInt(harga);
            }
            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);" /> Ayam Goreng Rp. 5.000</label><br />
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);" /> Tempe Goreng Rp. 5.00</label><br />
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);" /> Telur Dadar Rp. 2.500</label><br />
    <strong>Total Bayar: Rp. <input id="total" type="text" /></strong>
</body>
</html>
```



https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/efdf2394-0a7b-4623-a2d9-06c5468ca067



## Pertanyaan dan Tugas
**1. Buat script untuk melakukan `validasi` pada isian form**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulir Validasi</title>

    <!-- my styles css -->
    <link rel="stylesheet" href="style.css">
    <script>
        function validateForm() {
            // Dapatkan referensi ke elemen-elemen formulir
            var nama = document.forms["myForm"]["nama"].value;
            var email = document.forms["myForm"]["email"].value;

            // Lakukan validasi
            if (nama == "") {
                alert("Nama wajib diisi");
                return false;
            }

            if (email == "") {
                alert("Email wajib diisi");
                return false;
            }

            // Validasi apakah email sesuai dengan format yang benar
            var emailPattern = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/;

            if (!emailPattern.test(email)) {
                alert("Email tidak valid. Harap masukkan alamat email yang benar.");
                return false;
            }
        }
    </script>
</head>
<body>
    <h1>Formulir Validasi</h1>
    <div class="container">
        <form name="myForm" onsubmit="return validateForm()" method="post">
            <div class="input-group">
                <label for="nama"><img src="user (3).svg" class="label-img"></label>
                <input type="text" id="nama" name="nama" placeholder="Nama" class="input">
            </div>
            
            <div class="input-group">
                <label for="email"><img src="mail.svg" class="label-img"></label>
                <input type="text" id="email" name="email" placeholder="Email" class="input">
            </div>
            
    
            <input type="submit" value="Submit" class="btn">
        </form>
    </div>
    
</body>
</html>
```



https://github.com/tiaraputriiiiii/Lab5Web/assets/115775237/af9f87d9-9ce2-4127-af69-e57c8950c8d3



## Finish, Terima Kasih
