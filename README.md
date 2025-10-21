# Project Responsive Web Design using Bootstrap
## Date:18/10/2025

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Dribbble Clone - AIRA DARIO(25016155)</title>
  <link 
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" 
    rel="stylesheet" />
  <style>
    body {
       background-image: url("backgroundpic.png");
    }
    .navbar {
      background-color: #8f2323ff;
      border-bottom: 1px solid #3f0404ff;
    }

    .navbar-brand {
      font-size: 1.5rem;
      font-weight: bold;
      color: rgb(120, 0, 46) !important;
    }

     
    .banner {
      background: #2d2d2d;
      color: white;
      padding: 15px 0;
      text-align: center;
    }
    .banner .btn-signup {
      background-color: #c91d5fff;
      color: white;
      font-weight: 600;
      border: none;
    }

     
    .filter-bar {
      background-color: #082746ff;
      padding: 10px;
      display: flex;
      justify-content: center;
      gap: 20px;
      border-bottom: 1px solid rgb(2, 3, 101);
      flex-wrap: wrap;
    }
    .filter-bar select {
      border: none;
      font-size: 0.9rem;
      background: transparent;
      cursor: pointer;
    }

     
    .shot-card img {
      height: 200px;
      object-fit: cover;
      border-radius: 5px 5px 0 0;
      transition: transform 0.3s ease;
    }
    .shot-card:hover img {
      transform: scale(1.05);
    }
    .shot-card .card-body {
      padding: 10px;
    }
    .shot-stats {
      font-size: 0.85rem;
      color: #777;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

     
    .feature-section {
      background-color: #c2b607ff;
      padding: 50px 20px;
      text-align: center;
    }
    .feature-section h3 {
      font-weight: bold;
      margin-bottom: 20px;
    }

     
    footer {
      background-color: rgb(95, 1, 1);
      text-align: center;
      padding: 15px;
      font-size: 0.9rem;
      border-top: 1px solid rgb(189, 164, 3);
    }
  </style>
</head>
<body  >

   
  <nav class="navbar navbar-expand-lg">
    <div class="container">
      <a class="navbar-brand" href="#">DRIBBLE</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" 
              data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" 
              aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav me-3">
          <li class="nav-item"><a class="nav-link active" href="#">Shots</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Designers</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Teams</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Community</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Jobs</a></li>
        </ul>
        <form class="d-flex me-2">
          <input class="form-control form-control-sm" type="search" placeholder="Search" />
        </form>
        <a href="#" class="btn btn-outline-dark btn-sm me-2" data-bs-toggle="modal" data-bs-target="#loginModal">Sign in</a>
        <a href="#" class="btn btn-signup btn-sm" data-bs-toggle="modal" data-bs-target="#signupModal">Sign up</a>
      </div>
    </div>
  </nav>

  
  <div class="banner">
    <span>What are you working on? Dribbble is show and tell for designers.</span>
    <button class="btn btn-signup btn-sm ms-2" data-bs-toggle="modal" data-bs-target="#signupModal">Sign up</button>
  </div>

  
  <div class="filter-bar">
    <select>
      <option>Popular</option>
      <option>New</option>
      <option>Trending</option>
    </select>
    <select>
      <option>Shots</option>
      <option>Animations</option>
      <option>Illustrations</option>
    </select>
    <select>
      <option>Now</option>
      <option>This Week</option>
      <option>This Month</option>
    </select>
  </div>

   
  <div class="container my-4">
    <div class="row g-4">
       
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card shot-card shadow-sm">
          <img src="Screenshot 2025-10-15 221059.png" alt="Shot">
          <div class="card-body">
            <h6 class="mb-1 fw-semibold">Ethnic Fit</h6>
            <div class="shot-stats"><span>👁 4044</span><span>💬 125</span><span>❤ 1266</span></div>
          </div>
        </div>
      </div>
      
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card shot-card shadow-sm">
          <img src="Screenshot 2025-10-15 221033.png" alt="Shot">
          <div class="card-body">
            <h6 class="mb-1 fw-semibold">Campus Chronicles</h6>
            <div class="shot-stats"><span>👁 2404</span><span>💬 223</span><span>❤ 2360</span></div>
          </div>
        </div>
      </div>
 
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card shot-card shadow-sm">
          <img src="Screenshot 2025-10-15 221005.png" alt="Shot">
          <div class="card-body">
            <h6 class="mb-1 fw-semibold">Goofy Goodness</h6>
            <div class="shot-stats"><span>👁 3985</span><span>💬 170</span><span>❤ 2164</span></div>
          </div>
        </div>
      </div>
      
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card shot-card shadow-sm">
          <img src="Screenshot 2025-10-15 221123.png" alt="Shot">
          <div class="card-body">
            <h6 class="mb-1 fw-semibold">Back to the Benches</h6>
            <div class="shot-stats"><span>👁 2025</span><span>💬 69</span><span>❤ 1601</span></div>
          </div>
        </div>
      </div>
      <!-- Card 5 -->
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card shot-card shadow-sm">
          <img src="Screenshot 2025-10-21 122021.png" alt="Shot">
          <div class="card-body">
            <h6 class="mb-1 fw-semibold">Bouquet of Memories</h6>
            <div class="shot-stats"><span>👁 2179</span><span>💬 114</span><span>❤ 1581</span></div>
          </div>
        </div>
      </div>
     
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card shot-card shadow-sm">
          <img src= "Screenshot 2025-10-21 122117.png" alt="Shot">
          <div class="card-body">
            <h6 class="mb-1 fw-semibold">Friends & Frames</h6>
            <div class="shot-stats"><span>👁 1371</span><span>💬 119</span><span>❤ 627</span></div>
          </div>
        </div>
      </div>
       
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card shot-card shadow-sm">
          <img src="Screenshot 2025-10-21 122437.png" alt="Shot">
          <div class="card-body">
            <h6 class="mb-1 fw-semibold">Golden Days</h6>
            <div class="shot-stats"><span>👁 2728</span><span>💬 3</span><span>❤ 118</span></div>
          </div>
        </div>
      </div>
      
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card shot-card shadow-sm">
          <img src= "Screenshot 2025-10-21 122058.png" alt="Shot">
          <div class="card-body">
            <h6 class="mb-1 fw-semibold">Chill & Click</h6>
            <div class="shot-stats"><span>👁 1445</span><span>💬 225</span><span>❤ 2101</span></div>
          </div>
        </div>
      </div>
    </div>
  </div>

   
  <div class="feature-section">
    <div class="container">
      <h3>Join the world’s top creative community 🎨</h3>
      <p class="mb-4">Dribbble is where designers gain inspiration, feedback, community, and jobs. Get started today and grow your creative career.</p>
      <a href="#" class="btn btn-signup btn-lg" data-bs-toggle="modal" data-bs-target="#signupModal">Get Started</a>
    </div>
  </div>

  
  <div class="modal fade" id="signupModal" tabindex="-1" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title fw-bold">Create Your Account</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
        </div>
        <div class="modal-body">
          <form>
            <input class="form-control mb-2" type="text" placeholder="Full Name" required>
            <input class="form-control mb-2" type="email" placeholder="Email" required>
            <input class="form-control mb-3" type="password" placeholder="Password" required>
            <button class="btn btn-signup w-100">Sign Up</button>
          </form>
        </div>
      </div>
    </div>
  </div>

  
  <div class="modal fade" id="loginModal" tabindex="-1" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title fw-bold">Welcome Back</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
        </div>
        <div class="modal-body">
          <form>
            <input class="form-control mb-2" type="email" placeholder="Email" required>
            <input class="form-control mb-3" type="password" placeholder="Password" required>
            <button class="btn btn-signup w-100">Login</button>
          </form>
        </div>
      </div>
    </div>
  </div>

 
  <footer>
    © 2025  AIRA DARIO(25016155) — Built with ❤ Bootstrap | Inspired by Dribbble
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

## OUTPUT:
<img width="1920" height="1200" alt="Screenshot 2025-10-21 133727" src="https://github.com/user-attachments/assets/66a0e129-e52f-4c5d-b89a-b1b00f822f35" />


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
