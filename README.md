<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fiil Avı Oyunu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
        }
        #soru {
            font-size: 24px;
            margin: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 18px;
            margin: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Fiil Avı Oyunu</h1>
    <p id="soru">Cümledeki fiili bulun: "Ali hızlıca koştu."</p>
    
    <button onclick="kontrolEt('Ali')">Ali</button>
    <button onclick="kontrolEt('hızlıca')">hızlıca</button>
    <button onclick="kontrolEt('koştu')">koştu</button>
    
    <p id="sonuc"></p>

    <script>
        function kontrolEt(secim) {
            if (secim === "koştu") {
                document.getElementById("sonuc").innerHTML = "Doğru! +10 puan";
                document.getElementById("sonuc").style.color = "green";
            } else {
                document.getElementById("sonuc").innerHTML = "Yanlış! Tekrar dene.";
                document.getElementById("sonuc").style.color = "red";
            }
        }
    </script>
</body>
</html>
