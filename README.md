समझ गया! आपने जो QR कोड भेजा है, उसे मैं डिपॉज़िट सेक्शन में जोड़ दूँगा ताकि वह हर बार डिपॉज़िट के लिए दिख सके। अब मैं उस QR कोड को डिपॉज़िट सेक्शन में एम्बेड कर रहा हूँ।

Updated Code (With Your QR Code)

1. HTML (index.html)

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Akash Lucky Winner - Color Trading</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>Akash Lucky Winner - Color Trading</h1>
        
        <!-- Deposit Section -->
        <h2>Deposit</h2>
        <div class="form">
            <label for="deposit-amount">Enter Deposit Amount:</label>
            <input type="number" id="deposit-amount" min="1">
            <button id="deposit-btn">Deposit</button>
        </div>

        <!-- QR Code Section -->
        <div id="qr-deposit">
            <h3>Scan to Deposit</h3>
            <img src="QRCode.png" alt="Deposit QR Code" style="width: 150px; height: 150px;">
        </div>

        <h2>Trade Section</h2>
        <div class="form">
            <label for="color">Choose Color:</label>
            <select id="color">
                <option value="red">Red</option>
                <option value="green">Green</option>
                <option value="white">White</option>
            </select>
        </div>

        <div class="form">
            <label for="size">Choose Size:</label>
            <select id="size">
                <option value="small">Small</option>
                <option value="big">Big</option>
            </select>
        </div>

        <div class="form">
            <label for="number">Choose Number (1 to 9):</label>
            <input type="number" id="number" min="1" max="9">
        </div>

        <div class="form">
            <label for="amount">Enter Amount to Trade:</label>
            <input type="number" id="amount" min="1">
        </div>

        <button id="submit-btn">Submit Trade</button>

        <h2>Trade Results</h2>
        <div id="result"></div>
        <div id="winner"></div>
    </div>
    <script src="script.js"></script>
</body>
</html>
