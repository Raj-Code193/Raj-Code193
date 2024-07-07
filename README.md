<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>QR Code Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        .input-container {
            margin-bottom: 20px;
        }
        input {
            padding: 10px;
            font-size: 16px;
            width: 300px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
        }
        #qrcode {
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="input-container">
        <input type="text" id="text" placeholder="Enter text to generate QR Code">
        <button onclick="generateQRCode()">Generate QR Code</button>
    </div>
    <div id="qrcode"></div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
    <script>
        function generateQRCode() {
            const text = document.getElementById('text').value;
            if (text.trim() === "") {
                alert("Please enter some text");
                return;
            }
            document.getElementById('qrcode').innerHTML = ""; // Clear previous QR code
            new QRCode(document.getElementById("qrcode"), text);
        }
    </script>
</body>
</html>
- 👋 Hi, I’m @Raj-Code193
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Raj-Code193/Raj-Code193 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
