DOCTYPE htm<!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hoko Games</title>
  <style>
    body {
      font-family: tahoma, sans-serif;
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      color: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      margin: 0;
      direction: rtl;
    }
    .card {
      background: rgba(255, 255, 255, 0.05);
      padding: 20px;
      border-radius: 20px;
      text-align: center;
      width: 90%;
      max-width: 400px;
      box-shadow: 0 4px 20px rgba(0,0,0,0.3);
    }
    h1 {
      margin: 10px 0;
    }
    button {
      display: block;
      width: 100%;
      margin: 10px 0;
      padding: 12px;
      border: none;
      border-radius: 10px;
      font-size: 16px;
      cursor: pointer;
      color: white;
    }
    .telegram {
      background: #0088cc;
    }
    .instagram {
      background: #e1306c;
    }
    #qrcode {
      margin-top: 15px;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1 id="name"></h1>
    <p id="title"></p>
    <p id="location"></p>

    <button class="telegram" id="telegramBtn">رفتن به تلگرام</button>
    <button class="instagram" id="instagramBtn">رفتن به اینستاگرام</button>

    <p style="margin-top:15px;">اسکن کنید و همین صفحه را باز کنید:</p>
    <img id="qrcode" src="" alt="QR آدرس همین صفحه">
  </div>

  <script>
    const config = {
      name: "hoko",
      title: "Welcome to the world of Hoko games",
      location: "کرمانشاه، پاساژ قصر",
      telegramUsername: "hokogame",       // یوزرنیم تلگرام
      instagramUsername: "world_of_hoko"  // یوزرنیم اینستاگرام
    };

    document.getElementById("name").innerText = config.name;
    document.getElementById("title").innerText = config.title;
    document.getElementById("location").innerText = config.location;

    // باز کردن اپ تلگرام یا مرورگر
    document.getElementById("telegramBtn").onclick = () => {
      let appLink = "tg://resolve?domain=" + config.telegramUsername;
      let webLink = "https://t.me/" + config.telegramUsername;
      window.location.href = appLink;
      setTimeout(() => { window.open(webLink, "_blank"); }, 1000);
    };

    // باز کردن اپ اینستاگرام یا مرورگر
    document.getElementById("instagramBtn").onclick = () => {
      let appLink = "instagram://user?username=" + config.instagramUsername;
      let webLink = "https://instagram.com/" + config.instagramUsername;
      window.location.href = appLink;
      setTimeout(() => { window.open(webLink, "_blank"); }, 1000);
    };

    // ساخت QR با لینک همین صفحه
    document.getElementById("qrcode").src =
      "https://api.qrserver.com/v1/create-qr-code/?size=150x150&data=" + window.location.href;
  </script>
</body>
</html>l>

<html>
<head>
  <meta http-equiv="CONTENT-TYPE" content="text/html; charset=UTF-8">
  <link rel="stylesheet" href="styles/style.css"/>
  <title>Welcome</title>
</head>
<body>
  <h2 style="text-align: center;">
   
  </h2>
 برای برنده شدن نیاز به شکست‌های زیادی داری <br>
  <br>
</body>
</html>
