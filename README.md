<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Follow Frank</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #f9f9f9;
      padding: 50px;
    }
    .card {
      background: #fff;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      max-width: 400px;
      margin: auto;
    }
    button {
      margin-top: 20px;
      padding: 10px 20px;
      font-size: 16px;
      background: #007bff;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }
    button:hover {
      background: #0056b3;
    }
    #likeCount {
      font-size: 24px;
      color: #ff4081;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Support Frank!</h1>
    <p>Click below to like and follow Frank</p>
    <div>
      <p>❤️ Likes: <span id="likeCount">0</span></p>
      <button onclick="addLike()">Like</button>
    </div>
    <div>
      <button onclick="followFrank()">Follow</button>
    </div>
  </div>

  <script>
    let likes = 0;
    function addLike() {
      likes++;
      document.getElementById("likeCount").textContent = likes;
    }

    function followFrank() {
      alert("You're now following Frank! ✅");
    }
  </script>
</body>
</html>
