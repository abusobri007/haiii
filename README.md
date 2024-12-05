<!DOCTYPE html>
<html>
<meta charset='UTF-8'/><meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport'/><meta content='IE=edge' http-equiv='X-UA-Compatible'/><link href="https://feeldreams.github.io/withyou/style.css" rel="stylesheet" type="text/css" />
  
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Shippori+Antique:wght@400;700&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet">

  <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script>
  <script src="https://unpkg.com/typeit@8.7.0/dist/index.umd.js"></script>
  <script src="https://kit.fontawesome.com/4f3ce16e3e.js" crossorigin="anonymous"></script>
  
<head>
<title>Happy Birthday</title>
<link rel="icon" type="image/x-icon" href="https://malasid.github.io/favicon.png">
<!-- 
  Made with love by Rayys!
  
     Blog: https://PalingIT.com
     Instagram: @rayyarrr
     TikTok: @rayy4r
     Email: rayyar0703@gmail.com
     
  Thanks to all <3
-->
</head>
<body>
	
   <!-- Ganti Audio di sini -->
   <audio src="about-you.mp3" id="linkmp3" class="sembunyi"></audio>
   
   <div id="bodyblur">
     <!-- Wallpaper --><img src="https://feeldreams.github.io/wp2.jpeg" id="wallpaper"/><div id="beneranblur"></div>
   </div>
   
   <div id='Content'>

     <div id="kadoIn">
       <!-- Tombol Surat --><img src="https://feeldreams.github.io/kadoin.png"/>
     </div>
     <p id="ket">Klik Kadonya!</p>

     <div class="kumpulanstiker">
         <!-- Stiker untuk Konten -->
         <img src="https://feeldreams.github.io/peach6.gif" id="fotostiker"/>
         <img src="https://feeldreams.github.io/peach11.gif" id="fotostiker2"/>
         <img src="https://feeldreams.github.io/peachhug.gif" id="fotostiker3"/>
     </div>
     <p id="halo" class="halo">Haiii NiNa Cantikkkk!</p>
     <!-- Konten Pesan Setelah Aksi -->
     <p id="halo2" class="halo sty2">Munduran dikit cantiknya kelewatan🌟</p>
     <p id="halo3" class="halo sty3">Semoga tuhan selalu melindungi senyummu yang manis itu wkwk!</p>
     <p id="tanggal" class="halo sty3"></p>
     <!-- Konten Pesan Akhir -->
     <p id="kalimatbawah">Aku adalah orang yang selalu senang melihat mu baik baik sajaa ❤️</p> 
     <p id="kalimatbawah2" class="sembunyi">Tetaplah tersenyum manis seperti itu ❤️</p> 
     <p id="kalimatbawah3" class="sembunyi">Apapun yang berkaitan dengan mu aku selalu menyukainnya  ❤️</p>
       
     <div><blockquote id='bq' data-text='&#9829;'>

       <!-- Konten Pembukaan -->
       <p id="kalimat">Hai, aku cuman mau bilang.</p>
       <p id="kalimatb"> Setelah melewati semua kelelahan hari hari sebelumnya. 💪</p>
       <p id="kalimatc">Janagan lupa cari kesenangan kesenangan yang membuat kamu ingin hidup sehari lagi dan sehari lagi. 😊</p>
       <p id="kalimatd">Bumi ini luas sekali ,tapi untungnya kita ketemu wkwk .</p>
       <p id="kalimate">Jangan lupa untuk selalu tersenyum ya cantikkkkkk! 😊</p>
       <p id="kalimatf">Klik LOVE di Samping Kiri ya!</p>
       
       <p id="opsL">Klik untuk Lanjut</p>
       
     </blockquote></div>

     <!-- Tombol Kirim Pesan -->
     <div id="Tombol"><a id="By">&#128140; Balas</a></div>

     <!-- Pesan yang dikirim ke WhatsApp -->
     <span id="pesanWA" class="sembunyi"></span>
     
   </div>

<!-- Jangan Edit Bagian Ini --><script>
  const body = document.querySelector("body"); const style = document.createElement('style'); var today = new Date();var dd = String(today.getDate()).padStart(2, '0');var mm = String(today.getMonth() + 1).padStart(2, '0');var yyyy = today.getFullYear();const monthNames = ["Januari", "Februari", "Maret", "April", "Mei", "Juni", "Juli", "Agustus", "September", "Oktober", "November", "Desember"];today = dd + ' ' + monthNames[today.getMonth()] + ' ' + yyyy; inikuis=0;ftganti=0;flag=1;flagg=1;fungsi=0;ftfungsi=0;fungsiAwal=0;fungsitimer=0;vketikhalo=halo.innerHTML;halo.innerHTML = "";vketikhalo2=halo2.innerHTML;halo2.innerHTML = "";pesanwhatsapp = pesanWA.innerHTML;deffotostiker=fotostiker.src;Content.style = "opacity:1;margin-top:16vh;";
  audio = new Audio('' + linkmp3.src);tanggal.innerHTML="- " + today + " -"; function createHeart() {const heart = document.createElement("div"); heart.className = "fas fa-heart"; heart.style.left = (Math.random() * 90)+"vw"; heart.style.animationDuration = (Math.random()*3)+2+"s"; body.appendChild(heart);} setInterval(function name(params) {var heartArr = document.querySelectorAll(".fa-heart"); if (heartArr.length > 100) {heartArr[0].remove()}},100);
</script>
<script src="https://malasid.github.io/html/anniv.js"></script>
<!-- Sampai Sini -->
</body>
</html>
