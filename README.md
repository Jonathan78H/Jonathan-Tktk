<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Jonathan Palomo - Descargar Videos TikTok HD</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Montserrat', sans-serif;
      background: linear-gradient(to right, #0f0f0f, #1a1a1a);
      color: white;
      text-align: center;
      padding: 0;
    }

    header {
      background: #111;
      padding: 40px 20px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.6);
    }

    header h1 {
      font-size: 3em;
      margin: 0;
      color: #ff2d55;
    }

    header p {
      color: #bbb;
      font-size: 1.2em;
      margin-top: 10px;
    }

    .container {
      max-width: 600px;
      margin: 60px auto;
      padding: 20px;
      background: #1f1f1f;
      border-radius: 12px;
      box-shadow: 0 0 15px rgba(255, 45, 85, 0.2);
    }

    input[type="text"] {
      width: 100%;
      padding: 15px;
      font-size: 16px;
      border: none;
      border-radius: 8px;
      margin-bottom: 20px;
      background: #2a2a2a;
      color: white;
    }

    input::placeholder {
      color: #aaa;
    }

    button {
      padding: 15px 30px;
      font-size: 16px;
      background-color: #ff2d55;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    button:hover {
      background-color: #e0264a;
    }

    .note {
      color: #888;
      font-size: 0.9em;
      margin-top: 20px;
    }

    footer {
      margin-top: 80px;
      padding: 20px;
      font-size: 0.9em;
      background: #111;
      color: #666;
    }

    .spinner {
      display: none;
      margin: 20px auto;
      border: 6px solid #333;
      border-top: 6px solid #ff2d55;
      border-radius: 50%;
      width: 40px;
      height: 40px;
      animation: spin 1s linear infinite;
    }

    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 2.2em;
      }

      .container {
        margin: 40px 20px;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Jonathan Palomo</h1>
    <p>Descarga videos de TikTok en HD sin anuncios</p>
  </header>

  <div class="container">
    <input type="text" id="tiktokURL" placeholder="Pega aquí el enlace del video de TikTok" />
    <button onclick="descargarVideo()">Descargar Video</button>
    <div class="spinner" id="spinner"></div>
    <p class="note">Alta calidad, sin marcas de agua, sin interrupciones.</p>
  </div>

  <footer>
    &copy; 2025 Jonathan Palomo. Proyecto personal. No afiliado con TikTok.
  </footer>

  <script>
    function descargarVideo() {
      const url = document.getElementById("tiktokURL").value.trim();
      const spinner = document.getElementById("spinner");

      if (!url || !url.includes("tiktok.com")) {
        alert("Por favor, ingresa un enlace válido de TikTok.");
        return;
      }

      spinner.style.display = "block";

      // Aquí podrías integrar una API real
      setTimeout(() => {
        spinner.style.display = "none";
        alert("¡Descarga simulada completada!\n\n(Si tienes una API, aquí va el enlace de descarga real.)");

        // Ejemplo de redirección a una API externa:
        // window.location.href = `https://api-ejemplo.com/download?url=${encodeURIComponent(url)}`;
      }, 2500);
    }
  </script>

</body>
</html>
