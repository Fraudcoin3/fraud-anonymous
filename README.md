<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fraud-Anonymous</title>
    <style>
        body {
            background-color: black;
            color: white;
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            text-align: center;
        }
        h1 {
            font-size: 4rem;
            font-weight: bold;
        }
        .upload-container {
            margin-top: 20px;
        }
        input, button {
            margin: 10px;
            padding: 10px;
            font-size: 1rem;
        }
    </style>
</head>
<body>
    <h1>Fraud-Anonymous</h1>
    <div class="upload-container">
        <input type="file" id="imageUpload" accept="image/*">
        <input type="text" id="memeText" placeholder="Enter your meme text">
        <button onclick="generateMeme()">Create Meme</button>
    </div>
    <script>
        function generateMeme() {
            const imageInput = document.getElementById('imageUpload');
            const memeText = document.getElementById('memeText').value;
            
            if (imageInput.files.length === 0) {
                alert('Please upload an image.');
                return;
            }
            
            alert(`Generating meme with text: "${memeText}"`);
        }
    </script>
</body>
</html>
