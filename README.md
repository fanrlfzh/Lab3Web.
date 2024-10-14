#membuat List
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HTML Lanjutan</title>
</head>
<body>
<header>
<h1>Membuat List</h1>
</header>
</body>
</html>

#membuat Ordered List
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
    <li>Pemrograman Web</li>
    <li>Sistem Informasi</li>
    <li>Basis Data 2</li>
    </ol>
    </section>
![Screenshot (227)](https://github.com/user-attachments/assets/72703790-433b-421e-a492-4f5dc847ca5a)


#membuat Unordered List
<section id="unorder-list">
        <h2>Unordered List</h2>
        <ul type="square">
        <li>Jaringan Komputer</li>
        <li>Struktur Data</li>
        <li>Algoritma &amp; Pemrograman</li>
        </ul>
        </section>
        ![Screenshot (228)](https://github.com/user-attachments/assets/467d8434-aa54-4aea-8efb-75dd9091c73d)


#membuat Description List
<section id="unorder-list">
            <h2>Description List</h2>
            <dl>
            <dt>Fakultas Teknik</dt>
            <dd>Teknik Industri</dd>
            <dd>Teknik Informatika</dd>
            <dd>Teknik Lingkungan</dd>
            <dt>Fakultas Ekonomi dan Bisnis</dt>
            <dd>Akuntansi</dd>
            <dd>Manajemen</dd>
            <dd>Bisnis Digital</dd>
            </dl>
            </section>
            ![Screenshot (229)](https://github.com/user-attachments/assets/dba9f751-37d4-41b3-8f61-fb70e963d6fc)


#membuat Tabel
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HTML Lanjutan</title>
</head>
<body>
<header>
<h1>Membuat Table</h1>
</header>
</body>
</html>
<table border="1" cellpadding="4" cellspacing="0">
<thead>
<tr>
<th>No.</th>
<th>Fakultas</th>
<th>Program Studi</th>
</tr>
</thead>
<tbody>
<tr>
<td>1.</td>
<td>Teknik</td>
<td>Teknik Informatika</td>
</tr>
<tr>
<td>2.</td>
<td>Teknik</td>
<td>Teknik Industri</td>
</tr>
<tr>
<td>3.</td>
<td>Teknik</td>
<td>Teknik Lingkungan</td>
</tr>
</tbody>
</table>
![Screenshot (231)](https://github.com/user-attachments/assets/65c29d47-5027-4e1c-b4c6-9bf29fd8051d)


#mengatur Margin dan Padding
<table border="1" cellpadding="4" cellspacing="0">
![Screenshot (233)](https://github.com/user-attachments/assets/7d68d7a9-7092-4e90-abe4-f873a4b76983)


#menggabungkan Sel Data
<table border="1" cellpadding="6" cellspacing="0">
<thead>
<tr>
<th>No.</th>
<th>Fakultas</th>
<th>Program Studi</th>
</tr>
</thead>
<tbody>
<tr>
<td>1.</td>
<td rowspan="3">Teknik</td>
<td>Teknik Informatika</td>
</tr>
<tr>
<td>2.</td>
<td>Teknik Industri</td>
</tr>
<tr>
<td>3.</td>
<td>Teknik Lingkungan</td>
</tr>
</tbody>
</table>
![Screenshot (234)](https://github.com/user-attachments/assets/15926c7a-3c43-4071-99c1-d6e06a156b3e)


#membuat Form
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>HTML Lanjutan</title>
</head>
<body>
<header>
<h1>Membuat Form</h1>
</header>
</body>
</html>

<form action="proses.php" method="post">
    <fieldset>
    <legend>Data Pelanggan</legend>
    <p>
    <label for="nama">Nama</label>
    <input type="text" id="nama" name="nama">
    </p>
    <p>
    <label for="alamat">Alamat</label>
    <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
    </p>
    <p>
    <label>Jenis Kelamin</label>
    <input id="jk_l" type="radio" name="kelamin" value="L" /><label
    for="jk_l">Laki-laki</label>
    <input id="jk_p" type="radio" name="kelamin" value="P" /><label
    for="jk_p">Perempuan</label>
</p>
<p><input type="submit" value="Login"></p>
</fieldset>
</form>
![Screenshot (236)](https://github.com/user-attachments/assets/e5ccce81-e638-4a11-9823-090f2c33022e)


#menambahkan Style pada Form
<style>
    form p > label {
    display: inline-block;
    width: 100px;
    }
    form input[type="text"], form textarea {
    border: 1px solid #197a43;
    }
    form input[type="submit"] {
    border: 1px solid #197a43;
    background-color: #197a43;
    color: #ffffff;
    font-weight: bold;
    padding: 5px 15px;
    }
    </style>
    ![Screenshot (238)](https://github.com/user-attachments/assets/be203445-3f2e-44a9-b514-cea4b796e3cd)

#memvalidasi Dokumen
![Screenshot (243)](https://github.com/user-attachments/assets/ac46ddd7-008e-41b9-b2bb-f84e59518129)


Pertanyaan dan Tugas
1. Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form with Dropdown and Listbox</title>
</head>
<body>
    <h2>Form with Dropdown and Listbox</h2>

    <form action="/submit" method="post">
        <!-- Dropdown menu -->
        <label for="dropdown">Choose an option:</label>
        <select id="dropdown" name="dropdown">
            <option value="option1">Option 1</option>
            <option value="option2">Option 2</option>
            <option value="option3">Option 3</option>
        </select>
        <br><br>

        <!-- Listbox with multiple selection -->
        <label for="listbox">Select multiple options:</label>
        <select id="listbox" name="listbox[]" multiple size="5">
            <option value="optionA">Option A</option>
            <option value="optionB">Option B</option>
            <option value="optionC">Option C</option>
            <option value="optionD">Option D</option>
            <option value="optionE">Option E</option>
        </select>
        <br><br>

        <!-- Submit button -->
        <input type="submit" value="Submit">
    </form>
</body>
</html>
![Screenshot (239)](https://github.com/user-attachments/assets/35e51e45-a187-42b8-993c-6344b0757081)


