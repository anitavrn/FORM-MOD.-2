<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Registrasi</title>
    <style>
        label {
            display: inline-block;
            width: 190px; 
            vertical-align: top;
        }

        fieldset.kemampuan-dasar label {
            display: inline;
            width: 85%;
            margin-right: 2px; 
        }

        fieldset.kemampuan-dasar input {
            margin-right: 5px;
        }
    </style>
</head>
<body>
    <h1>Form Registrasi</h1>
    <form action="" method="post">
        <fieldset>
            <legend>Biodata</legend>
            <p>
                <label for="nama">Nama Mahasiswa</label>
                <span>:</span>
                <input type="text" id="nama" name="nama_mahasiswa" placeholder="Nama anda"/>
            </p>
            <p>
                <label for="nim">No Induk Mahasiswa (NIM)</label>
                <span>:</span>
                <input type="text" id="nim" name="nim" placeholder="123456789"/>
            </p>  
            <p>
                <label for="alamat">Alamat Mahasiswa</label>
                <span>:</span>
                <textarea id="alamat" name="alamat_mahasiswa" rows="4" placeholder="Alamat Anda"></textarea>
            </p> 
            <p>
                <label>Tanggal Lahir</label>
                <span>:</span>
                <select name="tanggal_lahir_hari">
                    <option value="01">01</option>
                    <option value="02">02</option>
                    <!-- Add other days here -->
                    <option value="31">31</option>
                </select>
                <select name="tanggal_lahir_bulan">
                    <option value="Januari">Januari</option>
                    <option value="Februari">Februari</option>
                    <option value="Maret">Maret</option>
                    <!-- Add other months here -->
                    <option value="Desember">Desember</option>
                </select>
                <select name="tanggal_lahir_tahun">
                    <option value="1990">1990</option>
                    <!-- Add other years here -->
                    <option value="2006">2006</option>
                </select>
            </p>
            <p>
                <label>Jenis Kelamin</label>
                <span>:</span>
                <label for="pria"><input type="radio" id="pria" name="jenis_kelamin" value="Pria"/> Pria</label>
                <label for="wanita"><input type="radio" id="wanita" name="jenis_kelamin" value="Wanita"/> Wanita</label>
            </p>
            <p>
                <label for="foto">Upload Foto</label>
                <span>:</span>
                <input type="file" id="foto" name="foto" accept="image/*"/>
            </p>
            <p>
                <label for="perguruan_tinggi">Perguruan Tinggi</label>
                <span>:</span>
                <input type="text" id="perguruan_tinggi" name="perguruan_tinggi" placeholder="Nama perguruan tinggi"/>
            </p>
        </fieldset>
        
        <fieldset>
            <legend>Info Akun</legend>
            <p>
                <label for="email">Email</label>
                <span>:</span>
                <input type="email" id="email" name="email" placeholder="Email Anda"/>
            </p>
            <p>
                <label for="username">Username</label>
                <span>:</span>
                <input type="text" id="username" name="username" placeholder="Username Anda"/>
            </p>
            <p>
                <label for="password">Password</label>
                <span>:</span>
                <input type="password" id="password" name="password" placeholder="Password Anda"/>
            </p>
            <p>
                <label for="confirm_password">Ulangi Password</label>
                <span>:</span>
                <input type="password" id="confirm_password" name="confirm_password" placeholder="Ulangi password"/>
            </p>
        </fieldset>
        
        <fieldset class="kemampuan-dasar">
            <legend>Kemampuan Dasar</legend>
            <p>
                <input type="checkbox" name="html" value="HTML" id="html"><label for="html">HTML</label>
                <input type="checkbox" name="css" value="CSS" id="css"><label for="css">CSS</label>
                <input type="checkbox" name="javascript" value="JavaScript" id="javascript"><label for="javascript">JavaScript</label>
                <input type="checkbox" name="php" value="PHP" id="php"><label for="php">PHP</label>
                <input type="checkbox" name="mysql" value="MySQL" id="mysql"><label for="mysql">MySQL</label>
                <input type="checkbox" name="laravel" value="Laravel" id="laravel"><label for="laravel">Laravel</label>
                <input type="checkbox" name="react_native" value="React Native" id="react_native"><label for="react_native">React Native</label>
            </p>
        </fieldset>
        
        <p>
            <input type="reset" value="Reset">
            <input type="submit" value="Simpan">
        </p>
    </form>
</body>
</html>
