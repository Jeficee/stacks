<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Photographer Profile</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 30px;
      line-height: 1.6;
    }
    .container {
      border: 1px solid #ccc;
      padding: 20px;
      max-width: 900px;
      margin: auto;
    }
    .header {
      display: flex;
      justify-content: space-between;
    }
    .profile {
      display: flex;
    }
    .profile img {
      width: 150px;
      height: 150px;
      border: 2px solid #999;
      margin-right: 20px;
      background-color: #eee;
    }
    .info {
      flex-grow: 1;
    }
    .info h1 {
      margin-top: 0;
    }
    .categories {
      text-align: right;
    }
    .categories h4 {
      margin: 0 0 10px 0;
    }
    .media {
      display: flex;
      margin-top: 20px;
      gap: 20px;
    }
    .media-item {
      flex: 1;
      text-align: center;
      border: 1px solid #aaa;
      padding: 10px;
      background-color: #f0f0f0;
      height: 120px;
    }
    .attachments {
      margin-top: 20px;
    }
    .attachments ul {
      list-style: none;
      padding-left: 0;
    }
    .attachments a {
      color: blue;
      text-decoration: underline;
      display: block;
      margin-bottom: 5px;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="header">
      <div class="profile">
        <img src ="https://feu.instructure.com/files/26444849/download?download_frd=1&verifier=t6T5RjsZUu6NNkW37OSxK2y4ljkw6yBbGs8QThG6">
        <div class="info">
          <h1>Marco Angelo M. Catalonia</h1>
          <p>Urbano Velasco Ave., Pinagbuhatan<br>
          Pasig City<br>
          Metro Manila, Philippines</p>
          <p>Email: <a href="mailto:firstname@surname.com">202411009@fit.edu.ph</a><br>
          Telephone: 0901 955 3705</p>
        </div>
      </div>
    </div>

    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi consectetur nibh feugiat urna elementum facilisis. Nullam diam arcu, lobortis ut tincidunt vel, suscipit quis lectus. Praesent interdum sapien in nisi tempor vestibulum. Mauris nec mauris sapien. Nam laoreet nisi non magna iaculis vitae convallis lorem porttitor.</p>

    

    <div class="media">
      <div class="media-item">Audio/Video</div>
      <div class="media-item">Image Gallery</div>
      <div class="attachments">
        <strong>Attachments</strong>
        <ul>
          <li><a href="#">Lorem ipsum dolor sit amet</a></li>
          <li><a href="#">Lorem ipsum dolor sit amet</a></li>
          <li><a href="#">Lorem ipsum dolor sit amet</a></li>
          <li><a href="#">Lorem ipsum dolor sit amet</a></li>
        </ul>
      </div>
    </div>
  </div>
</body>
</html>
