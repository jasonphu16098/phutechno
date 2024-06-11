<!DOCTYPE html>
<html>
<head>
   <title>Menu</title>
   <style type="text/css">
         body {
            background: #f0f0f0;
            font-family: Arial, sans-serif;
            color: #333;
            margin: 0;
            padding: 0;
         }
         .nav {
            background: rgba(51, 51, 51, 0.5); /* Giảm opacity để làm mờ thanh chứa nội dung */
            display: flex;
            height: 60px;
            align-items: center;
            justify-content: space-between;
            padding: 0 2em;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            z-index: 10; /* Đảm bảo thanh điều hướng ở phía trước video */
            position: relative;
         }
         #logo {
            color: rgb(224, 240, 238);
            font-size: 24px;
            text-decoration: none;
         }
         
         .menu {
            display: flex;
            align-items: center;
            justify-content: flex-end;
            flex: 1;
            margin-right: 2em;
         }
         .menu li {
            list-style: none;
            position: relative;
            margin-left: 20px; /* Khoảng cách giữa các mục menu */
         }
         .menu li a {
            display: block;
            padding: 0 20px;
            height: 60px;
            line-height: 60px;
            color: white;
            border: 2px solid transparent;
            transition: border 0.3s, background-color 0.3s, color 0.3s;
            text-align: center;
            text-decoration: none;
         }
         .menu li a:hover {
            border: 2px solid #ff69b4;
            background-color: #ff69b4;
            color: #333;
         }
         .menu_down {
            background: rgba(85, 85, 85, 0.5); /* Giảm opacity để làm mờ menu con */
            position: absolute;
            top: 60px;
            left: 0;
            width: 200px;
            display: none;
            flex-direction: column;
            padding: 0; /* Remove padding to prevent extra spacing */
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Add a subtle shadow for a more professional look */
            z-index: 20; /* Đảm bảo menu con ở phía trước video */
         }
         .menu_down li {
            text-align: center;
            padding: 10px 0; /* Giảm padding để làm cho nội dung nằm chính giữa */
         }
         .menu_down li a {
            color: white;
            text-decoration: none;
            transition: background-color 0.3s, color 0.3s;
         }
         .menu_down li a:hover {
            background-color: rgba(255, 105, 180, 0.5); /* Giảm opacity để làm mờ màu nền khi hover */
            color: #333;
         }
         .menu .menu_link:hover .menu_down {
            display: flex;
         }
         #hinh_anh_trang_chu {
            text-align: center;
         }
         .video-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100vh;
            overflow: hidden;
            z-index: -1; /* Đặt video ở phía sau tất cả các phần tử khác */
         }
         .video-container video {
            width: 100%;
            height: 100%;
            object-fit: cover;
         }
         .content {
            position: relative;
            z-index: 1;
            color: white;
            text-align: center;
            padding: 20px;
         }
      

   </style>
</head>
<body>
   <div class="nav">
      <a href="link_logo" id="logo"><strong> 25/5_MΞMORY<sup>©</sup> </strong></a>
      <ul class="menu">
         <li><a href="link1">HOME</a></li>
         <li><a href="link2">INTRODUCE</a></li>
         <li class="menu_link">
            <a href="link3">LOVE</a>
            <ul class="menu_down">
              <li><a href="LINK_LK">Part 1</a></li>
              <li><a href="LINK_LK2">Part 2</a></li>
              <li><a href="LINK_LK3">Part 3</a></li>
            </ul>
         </li>
         <li><a href="link4">CONTACT</a></li>
         <li><a href="link5">Login | Sign up</a></li>
      </ul>
   </div>
   <div class="video-container">
      <video autoplay muted loop playsinline class="video">
          <source src="New Project ‐ Được tạo bằng Clipchamp.mp4" type="video/mp4">
          
      </video>
  </div>




   </body>
</html>
