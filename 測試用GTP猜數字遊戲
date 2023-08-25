<!DOCTYPE html>
<html>
<head>
    <title>猜數字遊戲</title>
    <style>
        /* 添加一些自定義的CSS樣式 */
        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }
        
        #guessInput {
            width: 150px; /* 調整輸入框寬度 */
            font-size: 18px; /* 調整字體大小 */
        }
        
        button {
            font-size: 18px; /* 調整按鈕字體大小 */
            padding: 10px 20px; /* 調整按鈕內邊距 */
        }
        
        #message {
            font-size: 20px; /* 調整消息文字大小 */
            margin-top: 20px; /* 添加一些頂部間距 */
        }
    </style>
</head>
<body>
    <h1>猜數字遊戲</h1>
    <p>猜一個1到100之間的數字。</p>
    <input type="number" id="guessInput" min="1" max="100">
    <button onclick="checkGuess()">猜！</button>
    <p id="message"></p>
    
    <script>
        // JavaScript代碼將在此處放置
        const targetNumber = Math.floor(Math.random() * 100) + 1;
        let attempts = 0;

        function checkGuess() {
            const guessInput = document.getElementById('guessInput');
            const message = document.getElementById('message');
            const userGuess = parseInt(guessInput.value);

            if (isNaN(userGuess)) {
                message.textContent = '請輸入有效的數字。';
            } else {
                attempts++;
                if (userGuess === targetNumber) {
                    message.textContent = `恭喜！你在 ${attempts} 次嘗試後猜對了數字 ${targetNumber}。`;
                    guessInput.disabled = true;
                } else if (userGuess < targetNumber) {
                    message.textContent = '再大一點！';
                } else {
                    message.textContent = '再小一點！';
                }
            }
        }
    </script>
</body>
</html>
