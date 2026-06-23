# PositioningInCSS
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>CSS Positioning Practice</title>
  <style>
    /* Part 1: Static */
    .static-box { 
      width: 100px; height: 100px; 
      background: lightblue; 
      margin: 10px; 
      position: static; 
    }
    .header, .main, .footer {
      position: static;
      padding: 10px;
      background: #ddd;
      margin: 5px;
    }

    /* Part 2: Relative */
    .relative-box {
      width: 120px; height: 120px;
      background: lightgreen;
      position: relative;
      left: 50px; top: 30px;
    }
    .relative-second {
      width: 120px; height: 120px;
      background: pink;
      position: relative;
      left: 100px; top: 50px;
    }
    .profile-card img {
      position: relative;
      top: -10px;
    }
    .navbar .logo {
      position: relative;
      left: 20px;
    }

    /* Part 3: Absolute */
    .container {
      position: relative;
      width: 200px; height: 200px;
      background: #eee;
      margin: 20px;
    }
    .container .box {
      position: absolute;
      top: 20px; left: 30px;
      width: 50px; height: 50px;
      background: red;
    }
    .badge {
      position: relative;
      display: inline-block;
    }
    .badge span {
      position: absolute;
      top: -10px; right: -10px;
      background: red; color: white;
      border-radius: 50%; padding: 5px;
    }
    .id-card {
      position: relative;
      width: 200px; height: 120px;
      border: 1px solid #333;
    }
    .id-card img {
      position: absolute;
      top: 5px; right: 5px;
      width: 50px; height: 50px;
    }
    .gallery {
      position: relative;
      display: inline-block;
    }
    .gallery span {
      position: absolute;
      top: 5px; left: 5px;
      background: green; color: white;
      padding: 2px 5px;
    }
    .product {
      position: relative;
      width: 200px; height: 200px;
      border: 1px solid #333;
    }
    .product span {
      position: absolute;
      top: 5px; right: 5px;
      background: orange; color: white;
      padding: 2px 5px;
    }
    .login-field {
      position: relative;
      margin: 10px;
    }
    .login-field input {
      padding-left: 30px;
    }
    .login-field i {
      position: absolute;
      left: 5px; top: 5px;
    }

    /* Part 4: Fixed */
    .contact-btn {
      position: fixed;
      bottom: 10px; right: 10px;
      background: blue; color: white;
      padding: 10px;
    }
    .fixed-header {
      position: fixed;
      top: 0; left: 0; right: 0;
      background: black; color: white;
      padding: 10px;
    }
    .whatsapp-btn {
      position: fixed;
      bottom: 20px; right: 20px;
      background: green; color: white;
      padding: 10px; border-radius: 50%;
    }
    .back-top {
      position: fixed;
      bottom: 50px; right: 20px;
      background: purple; color: white;
      padding: 10px;
    }

    /* Part 5: Sticky */
    .sticky-nav {
      position: sticky;
      top: 0;
      background: #444; color: white;
      padding: 10px;
    }
    .section-title {
      position: sticky;
      top: 0;
      background: #ccc;
      padding: 5px;
    }
    table.sticky-table {
      border-collapse: collapse;
      width: 100%;
    }
    table.sticky-table th {
      position: sticky;
      top: 0;
      background: #eee;
    }
    table.sticky-table td, th {
      border: 1px solid #333;
      padding: 5px;
    }
  </style>
</head>
<body style="margin-top:60px;">

  <!-- Part 1: Static -->
  <div class="static-box">Box 1</div>
  <div class="static-box">Box 2</div>
  <div class="static-box">Box 3</div>

  <div class="header">Header</div>
  <div class="main">Main Content</div>
  <div class="footer">Footer</div>

  <!-- Part 2: Relative -->
  <div class="relative-box">Relative Box</div>
  <div class="relative-second">Second Box</div>

  <div class="profile-card">
    <img src="profile.jpg" alt="Profile">
    <p>Profile Card</p>
  </div>

  <div class="navbar">
    <span class="logo">Logo</span> | Home | About
  </div>

  <!-- Part 3: Absolute -->
  <div class="container">
    <div class="box"></div>
  </div>

  <div class="badge">Cart <span>5</span></div>

  <div class="id-card">
    <img src="student.jpg" alt="Student">
    <p>Student ID Card</p>
  </div>

  <div class="gallery">
    <img src="image.jpg" alt="Gallery" width="200">
    <span>New</span>
  </div>

  <div class="product">
    <p>Product Card</p>
    <span>20% OFF</span>
  </div>

  <div class="login-field">
    <i>🔒</i>
    <input type="password" placeholder="Password">
  </div>

  <!-- Part 4: Fixed -->
  <div class="fixed-header">Fixed Header</div>
  <button class="contact-btn">Contact Us</button>
  <button class="whatsapp-btn">💬</button>
  <button class="back-top">Top</button>

  <!-- Part 5: Sticky -->
  <div class="sticky-nav">Sticky Navigation</div>

  <div style="height:600px;">
    <h3 class="section-title">Section 1</h3>
    <p>Content...</p>
    <h3 class="section-title">Section 2</h3>
    <p>Content...</p>
    <h3 class="section-title">Section 3</h3>
    <p>Content...</p>
  </div>

  <table class="sticky-table">
    <tr><th>ID</th><th>Name</th></tr>
    <tr><td>1</td><td>Alice</td></tr>
    <tr><td>2</td><td>Bob</td></tr>
    <tr><td>3</td><td>Charlie</td></tr>
    <!-- Add many rows to test sticky header -->
  </table>

</body>
</html>
