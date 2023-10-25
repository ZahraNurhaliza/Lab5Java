# Lab5Java

## Langkah-langkah Praktikum
Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.
```html
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
</html
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.1.png)


### Javascrip Dasar
Pemakaian Alert sebagai property window.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>alert Box</title>
</head>
<body>
    <script language="javascript"> 

        window.alert('ini merupakan pesan untuk anda');
        
    </script>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.2.png)


Pemakaian method dalam objek
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Script javascript</title>
</head>
<body>
    percobaan pemakaian javascript:<br>
    <script languange="javascript">

        document.write('selamat mencoba javascript<br>');
        document.write('semoga sukses');
        
    </script>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.3.png)


Pemakaian Prompt
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>pemasukan data</title>
</head>
<body>
    <script language="javascript">

        var nama = prompt("siapa nama anda?","masukan nama anda: ");
        document.write("hai, " + nama);

    </script>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.4.png)


Pembuatan fungsi dan cara pemanggilannya
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Contoh program javascript</title>
    <script language="javascript">
        function pesan(){
            alert('memanggil javascript lewat body onload')
        }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.5.png)


### Dasar Pemrograman Di Javascript
Operasi dasar aritmatika
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
        function test (val1, val2)
        {
            document.write("<br>"+"perkalian : val1 * val2"+"<br>")
            document.write(val1*val2)
            document.write("<br>"+"pembagian : val1 / val2"+"<br>")
            document.write(val1/val2)
            document.write("<br>"+"penjumlahan : val1 + val2"+"<br>")
            document.write(val1+val2)
            document.write("<br>"+"pengurangan : val1 - val2"+"<br>")
            document.write(val1-val2)
            document.write("<br>"+"modulus : val1 % val2"+"<br>")
            document.write(val1%val2)
        }
    </script>
</head>
<body>
    <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.6.png)


Seleksi kondisi (if..else)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>contoh if-else</title>
</head>
<body>
    <script language="javascript">
        var nilai = prompt('nilai 0 - 100: ',0);
        var hasil = " ";
        if (nilai >= 60)
        hasil = "Lulus";
        else
        hasil = "tidak lulus";
        document.write ('hasil: '+hasil);
    </script>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.7.png)


Penggunaan operator switch untuk seleksi kondisi
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
        function test ()
        {
            val1=window.prompt ('input nilai (1-5):')
            switch (val1)
            {
                case '1':
                    document.write('bilangan satu')
                    break
                case '2' :
                    document.write('bilangan dua')
                    break
                case '3':
                    document.write('bilangan tiga')
                    break
                case '4' :
                    document.write('bilangan empat')
                    break
                case '5':
                    document.write('bilangan lima')
                    break
                default :
                    document.write('bilangan lainnya')
            }
        }
    </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.8.png)


### Pembuatan Form
Form Input
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <script language="javascript">
        function test () {
            var val1= document.kirim.t1.value;
            if (val1%2==0)
                document.kirim.t1.value="bilangan genap"
            else
                document.kirim.t2.value="bilangan ganjil"
        }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="t1" size="20"> MERUPAKAN BIL <input type="text" name="t2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1"onclick=test()></p>
    </form>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.9.png)


Form Button.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Objek document</title>
</head>
<body>
    <script language="javascript">
    function ubahWarnaLB(warna){
        document.bgColor= warna;
    }
    function ubahWarnaLD(warna){
        document.fgColor= warna;
    }
    </script>

    <h1>tes</h1>
    <form>
        <input type="button" value="latar Belakang Hijau" onclick="ubahWarnaLB('green')">
        <input type="button" value="latar Belakang Putih" onclick="ubahWarnaLB('white')">
        <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('yellow')">
        <input type="button" value="Teks Biru" onclick="ubahWarnaLD('blue')">
    </form>
    <script language="javascript">
    
    document.write("Dimodifokasi terakhir pada " + document.lastModified);
    
    </script>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.10.png)


### HTML DOM
Pilihan menggunakan checkBox dengan perhitungan otomatis
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele){
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total): 0);
            var harga = 0 ;

            if (ele.checked) {
                harga = ele.value;
                total += parseInt(harga);
            } else {
                harga = ele.value;
                if (total > 0 )
                    total -= parseInt(harga);
            }
            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this); "/> Ayam Goreng Rp. 5000</label><br />
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this); "/> Tempe Goreng Rp. 500</label><br />
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this); "/> Telur Dadar Rp. 2.500</label><br />
    <strong> Total Bayar: Rp. <input id="total" type="text"/> </strong>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.11.png)


## Pertanyaan dan Tugas
1. Buat script untuk melakukan validasi pada isian form.
```html
<!DOCTYPE html>
<html>
<head>
  <title>Contoh Validasi Form dengan CSS</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
    }

    .container {
      background-color: #fff;
      max-width: 400px;
      margin: 0 auto;
      padding: 20px;
      border-radius: 5px;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      text-align: center;
    }

    .form-group {
      margin-bottom: 20px;
    }

    label {
      font-weight: bold;
    }

    input[type="text"], input[type="password"] {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      margin-bottom: 10px;
      border: 1px solid #ccc;
      border-radius: 3px;
    }

    input[type="submit"] {
      background-color: #4CAF50;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 3px;
      cursor: pointer;
    }

    input[type="submit"]:hover {
      background-color: #45a049;
    }

    .error {
      color: red;
      text-align: left;
    }
  </style>
  <script>
    function validateForm() {
      var nama = document.forms["myForm"]["nama"].value;
      var email = document.forms["myForm"]["email"].value;
      var password = document.forms["myForm"]["password"].value;
      var errorMessages = "";

      if (nama == "") {
        errorMessages += "Nama harus diisi.\n";
      }

      if (email == "" || email.indexOf('@') == -1 || email.indexOf('.') == -1) {
        errorMessages += "Email tidak valid.\n";
      }

      if (password.length < 8) {
        errorMessages += "Password harus minimal 8 karakter.\n";
      }

      var errorDiv = document.getElementById("error-message");
      errorDiv.textContent = errorMessages;

      if (errorMessages !== "") {
        errorDiv.style.display = "block";
        return false;
      }

      errorDiv.style.display = "none";
    }
  </script>
</head>
<body>
  <div class="container">
    <h2>Form Registrasi</h2>
    <form name="myForm" onsubmit="return validateForm()" method="post">
      <div class="form-group">
        <label for="nama">Nama:</label>
        <input type="text" name="nama" id="nama">
      </div>

      <div class="form-group">
        <label for="email">Email:</label>
        <input type="text" name="email" id="email">
      </div>

      <div class="form-group">
        <label for="password">Password:</label>
        <input type="password" name="password" id="password">
      </div>

      <input type="submit" value="Submit">
      <div class="error" id="error-message"></div>
    </form>
  </div>
</body>
</html>
```

![image](https://github.com/ZahraNurhaliza/Lab5Java/blob/main/screenshot/ss.12.png)

## SELESAI