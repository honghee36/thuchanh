<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>KHÁNH ĐÔNG LẠNH - Trái cây sạch nhập khẩu & nội địa</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
    <style>
        :root {
            --primary: #ff6b35;   /* cam tươi */
            --green: #2ecc71;
            --light: #f9f9f9;
            --dark: #222;
        }
        * { margin:0; padding:0; box-sizing:border-box; }
        body { font-family:'Segoe UI',Arial,sans-serif; line-height:1.6; color:#333; background:var(--light); }

        header {
            position:fixed; top:0; width:100%; background:white; box-shadow:0 2px 15px rgba(0,0,0,0.1);
            z-index:1000; padding:15px 5%; display:flex; justify-content:space-between; align-items:center;
        }
        .logo { font-size:28px; font-weight:800; color:var(--primary); }
        .logo span { color:var(--green); }
        nav a {
            margin:0 15px; text-decoration:none; color:var(--dark); font-weight:600;
            transition:0.3s;
        }
        nav a:hover { color:var(--primary); }

        .hero {
            height:100vh; background:linear-gradient(rgba(0,0,0,0.4),rgba(0,0,0,0.5)),
                        url('https://images.unsplash.com/photo-1619566636858-adf3ef7c6085?w=1600') center/cover no-repeat;
            display:flex; flex-direction:column; justify-content:center; align-items:center;
            text-align:center; color:white;
        }
        .hero h1 { font-size:68px; margin-bottom:15px; text-shadow:0 3px 10px rgba(0,0,0,0.6); }
        .hero p { font-size:24px; margin-bottom:30px; }
        .btn {
            padding:15px 40px; background:var(--primary); color:white; border:none; border-radius:50px;
            font-size:18px; cursor:pointer; transition:0.4s; text-decoration:none; display:inline-block;
        }
        .btn:hover { background:#e55a2b; transform:scale(1.05); }

        section { padding:100px 5% 80px; text-align:center; }
        h2 { font-size:42px; margin-bottom:60px; color:var(--dark); position:relative; display:inline-block; }
        h2::after { content:''; width:80px; height:4px; background:var(--primary); position:absolute; bottom:-15px; left:50%; transform:translateX(-50%); }

        .grid {
            display:grid; grid-template-columns:repeat(auto-fit, minmax(280px,1fr)); gap:30px; max-width:1400px; margin:0 auto;
        }
        .card {
            background:white; border-radius:15px; overflow:hidden; box-shadow:0 10px 30px rgba(0,0,0,0.1);
            transition:0.4s;
        }
        .card:hover { transform:translateY(-15px); box-shadow:0 20px 40px rgba(0,0,0,0.15); }
        .card img { width:100%; height:280px; object-fit:cover; }
        .info { padding:20px; }
        .info h3 { font-size:22px; margin:10px 0; color:var(--dark); }
        .price { font-size:26px; color:var(--primary); font-weight:800; }
        .old-price { text-decoration:line-through; color:#999; margin-left:10px; }
        .add-cart {
            margin-top:15px; padding:12px 25px; background:var(--green); color:white;
            border:none; border-radius:30px; cursor:pointer; font-weight:600;
        }

        .contact { background:var(--dark); color:white; padding:80px 5%; }
        .social a { color:white; font-size:28px; margin:0 15px; transition:0.3s; }
        .social a:hover { color:var(--primary); transform:translateY(-5px); }

        @media (max-width:768px){
            .hero h1{font-size:48px;} .hero p{font-size:18px;}
            nav {position:absolute; top:100%; left:0; width:100%; background:white; flex-direction:column; display:none;}
            nav.active{display:flex;}
            .menu-btn{display:block; font-size:24px; cursor:pointer;}
        }
    </style>
</head>
<body>

<header>
    <div class="logo">KHÁNH<span>ĐÔNG LẠNH</span></div>
    <nav>
        <a href="#home">Trang chủ</a>
        <a href="#products">Sản phẩm</a>
        <a href="#contact">Liên hệ</a>
        <i class="fas fa-shopping-cart" style="font-size:22px;"></i>
    </nav>
    <div class="menu-btn" onclick="document.querySelector('nav').classList.toggle('active')">
        <i class="fas fa-bars"></i>
    </div>
</header>

<section class="hero" id="home">
    <h1>Trái Cây Tươi Ngon<br>Giá Tốt Mỗi Ngày</h1>
    <p>Giao tận nơi trong 2 năm – Cam kết tươi sạch 36%</p>
    <a href="#products" class="btn">Xem ngay sản phẩm</a>
</section>

<section id="products">
    <h2>Sản Phẩm Nổi Bật</h2>
    <div class="grid">
        <!-- Thẻ 1 -->
        <div class="card">
            <img src="https://images.unsplash.com/photo-1601001435827-8b9fc7e20a13?w=800" alt="Cherry">
            <div class="info">
                <h3>Cherry Mỹ Nhập Khẩu</h3>
                <p class="price">450.000đ <span class="old-price">550.000đ</span></p>
                <button class="add-cart">Thêm vào giỏ</button>
            </div>
        </div>
        <!-- Thẻ 2 -->
        <div class="card">
            <img src="https://images.unsplash.com/photo-1560020308-9d1d5036e6f3?w=800" alt="Dưa lưới">
            <div class="info">
                <h3>Dưa Lưới Tiền Giang</h3>
                <p class="price">85.000đ/kg</p>
                <button class="add-cart">Thêm vào giỏ</button>
            </div>
        </div>
        <!-- Thẻ 3 -->
        <div class="card">
            <img src="https://images.unsplash.com/photo-1587049352848-01f937b6e0e4?w=800" alt="Táo">
            <div class="info">
                <h3>Vải THiều</h3>
                <p class="price">120.000đ/kg</p>
                <button class="add-cart">Thêm vào giỏ</button>
            </div>
        </div>
        <!-- Thẻ 4 -->
        <div class="card">
            <img src="https://images.unsplash.com/photo-1571575173700-afb9492e6a50?w=800" alt="Xoài">
            <div class="info">
                <h3>Cát Hòa Lộc</h3>
                <p class="price">65.000đ/kg</p>
                <button class="add-cart">Thêm vào giỏ</button>
            </div>
        </div>
        <!-- Thẻ 5 -->
        <div class="card">
            <img src="https://images.unsplash.com/photo-1622737133809-d95047f23220?w=800" alt="Nho mẫu đơn">
            <div class="info">
                <h3>Tỏi Nam Đinh </h3> 
                <p class="price">350.000đ/kg</p>
                <button class="add-cart">Thêm vào giỏ</button>
            </div>
        </div>
        <!-- Thẻ 6 -->
        <div class="card">
            <img src="https://images.unsplash.com/photo-1596591606975-276fa09c7f64?w=800" alt="Thanh long">
            <div class="info">
                <h3>Thanh Long Ruột Đỏ</h3>
                <p class="price">45.000đ/kg</p>
                <button class="add-cart">Thêm vào giỏ</button>
            </div>
        </div>
    </div>
</section>

<section class="contact" id="contact">
    <h2>Liên hệ đặt hàng ngay hôm nay</h2>
    <p style="font-size:20px; margin:20px 0;">
        Hotline/Zalo: <b>0909 123 456</b><br>
        Fanpage: <a href="https://www.facebook.com/tran.khanh.71489?locale=vi_VN" style="color:var(--primary)">facebook.com/freshfruit</a><br>
        Giao hàng toàn quốc – Thanh toán khi nhận hàng
    </p>
    <div class="social">
        <a href="#"><i class="fab fa-facebook"></i></a>
        <a href="#"><i class="fab fa-tiktok"></i></a>
        <a href="#"><i class="fab fa-instagram"></i></a>
    </div>
</section>

</body>
</html>
