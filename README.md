<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Foto Upload Formular</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      max-width: 600px;
      margin: 40px auto;
      padding: 20px;
      border: 1px solid #ccc;
      border-radius: 10px;
      background-color: #f9f9f9;
    }
    label {
      display: block;
      margin-top: 15px;
    }
    input, button {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      box-sizing: border-box;
    }
    button {
      background-color: #007bff;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    button:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>
  <h1>Foto-Upload</h1>
  <form 
    action="https://formspree.io/f/mldboyqj" 
    method="POST" 
    enctype="multipart/form-data"
  >
    <label for="name">Dein Name:</label>
    <input type="text" name="name" id="name" required>

    <label for="email">Deine E-Mail:</label>
    <input type="email" name="_replyto" id="email" required>

    <label for="file">Foto hochladen:</label>
    <input type="file" name="attachment" id="file" accept="image/*" required>

    <button type="submit">Absenden</button>
  </form>
</body>
</html>
