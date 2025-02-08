<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Combined Circle Slider</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" />
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet" />
  <script src="https://code.jquery.com/jquery-3.7.1.js"></script>
  <style>
    /* Social Icons & Navbar */
    .social-icons {
      display: flex;
      justify-content: flex-start;
      padding: 10px 20px;
      background-color: #007bff;
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 1000;
    }
    .social-icons a {
      text-decoration: none;
      color: #fff;
      margin-right: 15px;
      font-size: 17px;
    }
    .social-icons a:hover { 
      color: black; 
    }
    .call-icon {
      width: 20px;
      height: 20px;
      vertical-align: middle;
      margin-right: 5px;
    }
    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px 20px;
      background-color: #091127;
      margin-top: 50px;
    }
    .navbar-logo img { 
      height: 200px; 
      margin-left: 20px;
    }
    .search-container {
      display: flex;
      align-items: center;
      justify-content: center;
      flex-grow: 1;
    }
    .search-bar input {
      padding: 8px;
      font-size: 16px;
      width: 600px;
      border-radius: 15px 0 0 15px;
      border: 1px solid #fff;
    }
    .search-bar button {
      padding: 8px 15px;
      border: 1px solid #fff;
      background-color: #007bff;
      color: white;
      border-radius: 0 15px 15px 0;
      cursor: pointer;
    }
    .search-bar button:hover {
      background-color: #0056b3;
    }
    .menu-bar {
      background-color: #007bff;
      padding: 10px;
      text-align: center;
    }
    .menu-bar a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-size: 18px;
    }
    .menu-bar a i {
      margin-right: 5px;
    }
    .menu-bar a:hover { 
      color: black; 
    }
    .carousel-inner img {
      height: 550px;
      object-fit: cover;
    }
    h3 {
      text-align: center;
      padding-top: 28px;
    }
    p {
      text-align: center;
      font-weight: bold;
    }
    .card {
  overflow: hidden; /* Prevents image from overflowing */
  border-radius: 10px; /* Optional: adds rounded corners */
}

.card-img-top {
  transition: transform 0.3s ease-in-out;
}

.card-img-top:hover {
  transform: scale(1.1);
}

  </style>
</head>
<body>
  <!-- Social Icons -->
  <div class="social-icons">
    <a href="tel:+03700319890">
      <img src="https://icons.veryicon.com/png/o/miscellaneous/fs-icon/call-13.png" class="call-icon" alt="Call Icon"> 03700319890
    </a>
    <a href="#"><i class="fab fa-instagram"></i></a>
    <a href="#"><i class="fab fa-facebook"></i></a>
    <a href="#"><i class="fab fa-youtube"></i></a>
  </div>

<div  class="">
  <div class="navbar">
    <div class="navbar-logo">
      <img src="logo.jpg" alt="Logo">
    </div>
    <div class="search-container">
      <div class="search-bar">
        <input type="text" placeholder="I'm Looking for...">
        <button><i class="fas fa-search"></i></button>
      </div>
    </div>
  </div>
</div>
  <!-- Menu Bar -->
  <div class="menu-bar">
    <a href="#"><i class="fas fa-home"></i> Home</a>
    <a href="#"><i class="fas fa-store"></i> Shop</a>
    <a href="#"><i class="fas fa-shopping-cart"></i> Cart</a>
    <a href="#"><i class="fas fa-info-circle"></i> About</a>
  </div>


  <div id="carouselExampleFade" class="carousel slide carousel-fade" data-bs-ride="carousel">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="https://clopal.com/cdn/shop/files/Web_banner_1.png?v=1731572530&width=1500" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="https://clopal.com/cdn/shop/files/Web_banner_3.png?v=1731572753&width=1500" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="https://clopal.com/cdn/shop/files/Web-Banner-5.jpg?v=1731572548&width=1500" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="https://clopal.com/cdn/shop/files/Web_Banner_6.png?v=1731572795&width=1500" class="d-block w-100" alt="...">
      </div>
    </div>
    <a class="carousel-control-prev" href="#carouselExampleFade" role="button" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" href="#carouselExampleFade" role="button" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="onclick">Next</span>
    </a>
  </div>


  <!-- TODAY HOT DEALS -->
  <div>
    <h3>
      <b>
        TODAY HOT DEALS <i class="fas fa-fire"></i>
      </b>
    </h3>
  </div>

  <!-- Cards Grid (4 cards per row, 3 rows) -->
  <div class="container mt-4">
    <div class="row row-cols-1 row-cols-md-4 g-4">
      <!-- Card 1 -->
      <div class="col">
        <div class="card">
          <img src="https://clopal.com/cdn/shop/files/Wifi-Black-1-Gang.jpg?v=1738324505&width=360" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://clopal.com/cdn/shop/files/1-Fan-Remote-Control_f31d2d67-53fb-43a0-8793-67236fc6672f.webp?v=1738324369" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://clopal.com/cdn/shop/files/1-3_e6c5bea9-6831-46ae-803e-64502bf16da3.webp?v=1738324539" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://clopal.com/cdn/shop/files/clopal-ext-CP-138.webp?v=1738324473&width=360" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://powerdigitalmarketing.com/wp-content/uploads/2024/11/Paid-Search.png" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://powerdigitalmarketing.com/wp-content/uploads/2024/11/Paid-Search.png" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://powerdigitalmarketing.com/wp-content/uploads/2024/11/Paid-Search.png" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://powerdigitalmarketing.com/wp-content/uploads/2024/11/Paid-Search.png" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://powerdigitalmarketing.com/wp-content/uploads/2024/11/Paid-Search.png" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://powerdigitalmarketing.com/wp-content/uploads/2024/11/Paid-Search.png" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://powerdigitalmarketing.com/wp-content/uploads/2024/11/Paid-Search.png" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card">
          <img src="https://powerdigitalmarketing.com/wp-content/uploads/2024/11/Paid-Search.png" class="card-img-top" alt="Card image">
          <div class="card-body">
            <h5 class="card-title">PPC Campaigns</h5>
            <p class="card-text">We build PPC campaigns for sustainable growth.</p>
            <a href="#" class="btn btn-primary">Get a proposal</a>
          </div>
        </div>
      </div>
      
   
      <script>
        var myCarousel = document.querySelector('#carouselExampleFade');
        var carousel = new bootstrap.Carousel(myCarousel, {
          ride: 'carousel'
        });
      </script>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
