# kantin-berkah-ai 
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>KANTIN BERKAH AI</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      padding: 20px;
    }
    h1 {
      text-align: center;
      color: #2c3e50;
    }
    .menu-item {
      background-color: #fff;
      border-radius: 12px;
      padding: 15px;
      margin: 15px auto;
      max-width: 400px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      text-align: center;
    }
    .menu-item img {
      width: 100%;
      max-height: 200px;
      object-fit: cover;
      border-radius: 8px;
    }
    .menu-item h2 {
      margin: 10px 0 5px;
      font-size: 20px;
    }
    .menu-item p {
      color: #666;
      margin: 5px 0;
    }
    button {
      background-color: #28a745;
      color: white;
      padding: 10px 15px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      margin-top: 10px;
    }
    button:hover {
      background-color: #218838;
    }
    #namaInput {
      width: 100%;
      max-width: 400px;
      margin: 0 auto 20px;
      display: block;
      padding: 10px;
      font-size: 16px;
      border-radius: 6px;
      border: 1px solid #ccc;
    }
  </style>
</head>
<body>

<h1>KANTIN BERKAH AI</h1>
<input type="text" id="namaInput" placeholder="Masukkan Nama Kamu Dulu Ya 😊">

<div class="menu-item">
  <img src="https://i.ibb.co/x3KNn7L/dimsum.jpg" alt="Dimsum">
  <h2>Dimsum</h2>
  <p>Harga: Rp 2.500</p>
  <button onclick="pesan('Dimsum')">Pesan Sekarang</button>
</div>

<div class="menu-item">
  <img src="https://i.ibb.co/zPfs68R/papeda-puyuh.jpg" alt="Papeda Telur Puyuh">
  <h2>Papeda Telur Puyuh</h2>
  <p>Harga: Rp 2.000</p>
  <button onclick="pesan('Papeda Telur Puyuh')">Pesan Sekarang</button>
</div>

<div class="menu-item">
  <img src="https://i.ibb.co/zJQK2q9/papeda-ayam.jpg" alt="Papeda Telur Ayam">
  <h2>Papeda Telur Ayam</h2>
  <p>Harga: Rp 5.000</p>
  <button onclick="pesan('Papeda Telur Ayam')">Pesan Sekarang</button>
</div>

<script>
  function pesan(menu) {
    const nama = document.getElementById('namaInput').value.trim();
    if (!nama) {
      alert("Isi nama kamu dulu ya!");
      return;
    }
    const nomorWA = '6283861042607';
    const pesanWA = `Halo, saya (${nama}) mau pesan: ${menu}`;
    const link = `https://wa.me/${nomorWA}?text=${encodeURIComponent(pesanWA)}`;
    window.open(link, '_blank');
  }
</script>

</body>
</html>
