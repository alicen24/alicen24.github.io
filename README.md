
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>คำถามรักๆ</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            text-align: center;
            background-color: #000000;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            color: #ffffff;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: #ffffff;
            font-weight: 700;
        }

        .question {
            font-size: 1.5rem;
            margin: 20px;
            color: #ffffff;
        }

        .buttons {
            margin-top: 20px;
        }

        .btn {
            padding: 15px 30px;
            font-size: 18px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin: 10px;
            transition: all 0.3s ease;
            font-weight: 500;
        }

        .ok-kub {
            background-color: #4caf50;
            color: white;
        }

        .oh-friend {
            background-color: #f44336;
            color: white;
        }

        .result {
            margin-top: 30px;
            font-size: 1.5rem;
            color: #ffffff;
        }
    </style>
</head>
<body>

<h1>นี่ๆ มีอะไรจะถามหน่อย</h1>
<div class="question">คือว่างี้นะ แบบ คือนี่อยากถามว่า เอ่ออออออ.........แกอยากลองคุยกันแบบจริงจังกับเค้ามั้ยย>< หรือแกมีคนในใจแล้วมาบอกกันตรงๆได้ ยินดีนะ</div>

<div class="buttons">
    <button class="btn ok-kub" onclick="answer('ok')">OK kub</button>
    <button class="btn oh-friend" onclick="answer('friend')">Oh on just friend</button>
</div>

<div id="result" class="result"></div>

<script>
    function answer(response) {
        var resultDiv = document.getElementById("result");

        if (response === 'ok') {
            resultDiv.innerHTML = "<p>ค้าบ สัญญาว่าจะพยายามไม่ทำให้แกอึดอัดนะ</p>";
        } else {
            resultDiv.innerHTML = "<p>ไม่เป็นไร ยังไงก็เป็นเพื่อนกันอยู่แล้ว ไม่ต้องคิดมาก</p>";
        }
    }
</script>

</body>
</html>
