# broma-android
Broma Android
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Android Security</title>
<style>
  body {
    background:#0f172a;
    color:#e5e7eb;
    font-family: Arial, sans-serif;
    text-align:center;
    padding-top:60px;
  }
  .box{
    background:#020617;
    margin:auto;
    width:90%;
    max-width:400px;
    padding:20px;
    border-radius:12px;
    box-shadow:0 0 20px rgba(0,0,0,.6);
  }
  button{
    background:#22c55e;
    color:white;
    font-size:18px;
    padding:15px 30px;
    border:none;
    border-radius:10px;
    cursor:pointer;
    margin-top:25px;
  }
  button:hover{ background:#16a34a; }

  .screen{
    display:none;
    position:fixed;
    inset:0;
    z-index:9999;
    text-align:center;
    padding-top:35%;
  }

  #hackScreen{
    background:black;
    color:#ff3b3b;
    font-size:24px;
  }

  #finalScreen{
    background:#020617;
    color:white;
    font-size:24px;
  }
</style>
</head>
<body>

<div class="box">
  <h2>🤖 ANDROID SECURITY</h2>
  <p>Presiona para iniciar escaneo del sistema</p>
  <button onclick="startBroma()">Iniciar Escaneo</button>
</div>

<div class="screen" id="hackScreen">
  ⚠️ TU TELÉFONO HA SIDO HACKEADO ⚠️
  <br><br>
  <button onclick="deshackear()">Haz click para des‑hackear</button>
</div>

<div class="screen" id="finalScreen">
  😂 ES UNA BROMA 😂
  <br><br>
  <b>De tu amigo DYLAN</b>
  <br>
  🗣️🔥🔥🔥🔥🔥
</div>

<script>
function startBroma(){
  window.open("https://www.google.com", "_blank");
  document.getElementById("hackScreen").style.display = "block";
}

function deshackear(){
  document.getElementById("hackScreen").style.display = "none";
  document.getElementById("finalScreen").style.display = "block";
}
</script>

</body>
</html>
