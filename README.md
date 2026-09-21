html = r'''<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>🌻 Feliz día de las flores amarillas 🌻</title>
<style>
  *{box-sizing:border-box}
  body{
    margin:0; min-height:100vh; display:flex; align-items:center; justify-content:center;
    font-family:Arial,sans-serif; text-align:center;
    background:linear-gradient(135deg,#fff8b5,#ffd84d,#ffef8a);
    overflow:hidden;
  }
  .card{
    width:min(90%,520px); padding:35px 25px; border-radius:28px;
    background:rgba(255,255,255,.78); box-shadow:0 12px 35px rgba(120,85,0,.22);
    position:relative; z-index:2;
  }
  h1{color:#e5a900;margin:0 0 15px;font-size:2rem}
  p{color:#6b5200;font-size:1.1rem;line-height:1.6}
  .flowers{font-size:4rem; animation:float 2.5s ease-in-out infinite}
  .heart{font-size:2rem}
  @keyframes float{50%{transform:translateY(-10px)}}
  .petal{position:absolute;font-size:25px;animation:fall linear infinite;opacity:.8}
  @keyframes fall{from{transform:translateY(-10vh) rotate(0)}to{transform:translateY(110vh) rotate(360deg)}}
</style>
</head>
<body>
<div class="petal" style="left:8%;animation-duration:7s">🌼</div>
<div class="petal" style="left:25%;animation-duration:9s;animation-delay:2s">🌻</div>
<div class="petal" style="left:48%;animation-duration:8s;animation-delay:1s">🌼</div>
<div class="petal" style="left:70%;animation-duration:10s;animation-delay:3s">🌻</div>
<div class="petal" style="left:88%;animation-duration:7.5s;animation-delay:1.5s">🌼</div>

<div class="card">
  <div class="flowers">🌻🌼🌻</div>
  <h1>¡Feliz día de las flores amarillas! 💛</h1>
  <p>
    Que hoy esté lleno de alegría, buenos momentos
    y muchas flores amarillas. 🌻✨
  </p>
  <div class="heart">💛🌻💛</div>
</div>
</body>
</html>'''

path = "/mnt/data/flores_amarillas.html"
with open(path, "w", encoding="utf-8") as f:
    f.write(html)

print(f"[Descargar flores_amarillas.html](sandbox:{path})")
