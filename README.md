# Tailwindcss 

### Weird way to use Tailwindcss

```bash
 <head>
    <script src="https://unpkg.com/@tailwindcss/browser@4"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />
    <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
</head>
<body>
    <div class="@container">
    <nav class="bg-gray-900 text-white">
        <div class="container mx-auto px-4 flex justify-between items-center py-3">
            <a href="#" class="text-xl font-bold">NASA</a>
            <button class="md:hidden text-white focus:outline-none">
                ☰
            </button>
            <ul class="hidden md:flex space-x-4">
                <li><a href="#" class="hover:text-gray-400">Home</a></li>
                <li><a href="#" class="hover:text-gray-400">About</a></li>
                <li><a href="#" class="hover:text-gray-400">Contact</a></li>
            </ul>
        </div>
    </nav>

    <div class="container mx-auto px-6 mt-10">
        <div class="flex flex-col md:flex-row items-center">

            <div class="md:w-1/2 flex justify-center mx-4">
                <img style="border-radius: 50%;" src="https://www.nasa.gov/wp-content/themes/nasa/assets/images/default-thumbnail.jpg" 
                    class="w-full max-w-md rounded-lg shadow-lg" alt="nasa">
            </div>
            
            <div class="md:w-1/2 mt-6 md:mt-0">
                <h1 class="text-3xl font-bold">WELCOME TO NASA</h1>
                <p class="mt-4 text-gray-600">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut harum repudiandae sit eius! Quo animi earum impedit, laudantium quidem fugit ipsa ullam sunt, explicabo veniam non, minus molestiae natus dolorem eum aut rerum rem velit! Illo iusto sapiente, similique quis at dolorum nam eveniet doloremque esse voluptates officiis, maiores vitae?
                </p>
                <div class="mt-4">
                    <button class="bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-600">Explore</button>
                    <button class="bg-green-500 text-white px-4 py-2 rounded hover:bg-green-600 ml-2">Contact</button>
                </div>
            </div>
        </div>
    </div>
    
    <div class="container mx-auto grid grid-cols-1 md:grid-cols-3 gap-6 py-8">
        
        <div class="bg-white shadow-lg rounded-lg overflow-hidden">
            <img src="https://www.cronodon.com/images/mercury-3.gif" 
                 alt="Image" class="w-full h-48 object-cover">
            <div class="p-4">
                <h5 class="text-lg font-semibold">Card Title</h5>
                <p class="text-gray-600">Some description about this card.</p>
                <button class="mt-4 bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-600">Learn More</button>
            </div>
        </div>
    
        <div class="bg-white shadow-lg rounded-lg overflow-hidden">
            <img src="https://i.pinimg.com/originals/1a/a2/d5/1aa2d5fee3ea2e2af739959bf3911f3e.gif" 
                 alt="Image" class="w-full h-48 object-cover">
            <div class="p-4">
                <h5 class="text-lg font-semibold">Card Title</h5>
                <p class="text-gray-600">Some description about this card.</p>
                <button class="mt-4 bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-600">Learn More</button>
            </div>
        </div>
    </div>
    
    <div class="w-full max-w-4xl mx-auto">
        <div class="swiper mySwiper">
            <div class="swiper-wrapper">
                <!-- Slide 1 -->
                <div class="swiper-slide relative">
                    <img src="https://i.pinimg.com/736x/ab/76/c0/ab76c06b09e4a0812b653ba703e7c557.jpg" class="w-full h-[500] object-cover rounded-lg" alt="Slide 1">
                    <div class="absolute bottom-5 left-0 w-full text-center text-white bg-opacity-50 p-4">
                        <h5 class="text-lg font-bold">First slide label</h5>
                        <p>Some representative placeholder content for the first slide.</p>
                    </div>
                </div>
                <!-- Slide 2 -->
                <div class="swiper-slide relative">
                    <img src="https://image.slidesdocs.com/responsive-images/background/blue-beautiful-night-nature-galaxy-space-powerpoint-background_a1cc625475__960_540.jpg" class="w-full h-[500] object-cover rounded-lg" alt="Slide 2">
                    <div class="absolute bottom-5 left-0 w-full text-center text-white bg-opacity-50 p-4">
                        <h5 class="text-lg font-bold">Second slide label</h5>
                        <p>Some representative placeholder content for the second slide.</p>
                    </div>
                </div>
                <!-- Slide 3 -->
                <div class="swiper-slide relative">
                    <img src="https://ichef.bbci.co.uk/images/ic/480xn/p023hqw3.jpg" class="w-full h-[500] object-cover rounded-lg" alt="Slide 3">
                    <div class="absolute bottom-5 left-0 w-full text-center text-white bg-opacity-50 p-4">
                        <h5 class="text-lg font-bold">Third slide label</h5>
                        <p>Some representative placeholder content for the third slide.</p>
                    </div>
                </div>
            </div>
    
            <div class="swiper-button-next text-gray-800"></div>
            <div class="swiper-button-prev text-gray-800"></div>
    
            <div class="swiper-pagination"></div>


        </div>
    </div>
    
    
    <footer class="bg-gray-900 text-white text-center py-4 mt-10">
        <p>© 2024 My Website. All rights reserved.</p>
    </footer>
</div>
<script>
    document.addEventListener("DOMContentLoaded", function () {
        new Swiper(".mySwiper", {
            loop: true,
          
            pagination: {
                el: ".swiper-pagination",
                clickable: true,
            },
            navigation: {
                nextEl: ".swiper-button-next",
                prevEl: ".swiper-button-prev",
            },
        });
    });
</script>
</body>
```
### Output
![Screenshot from 2025-03-30 22-18-54](https://github.com/user-attachments/assets/cf78187b-e7a4-44c4-bd33-a58bf4d35391)

### Professional way to use Tailwindcss

Install dependencies

```bash
npm install -D tailwindcss postcss autoprefixer
```
Initialize 

```bash
npx tailwindcss init -p
```
configure file

```bash
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [ 
    "./index.html",     
    "./src/**/*.{js,jsx,ts,tsx}",],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

style.css

```bash
@tailwind base;
@tailwind components;
@tailwind utilities;

.container-wrapper {
    @apply container mx-auto px-6 mt-10;
}

nav {
    @apply bg-gray-900 text-white py-4;
}

.containerr {
    @apply flex justify-between items-center mx-auto px-6;
}

.logo {
    @apply text-2xl font-bold tracking-wide;
}

ul {
    @apply hidden md:flex gap-6; 
}

ul li {
    @apply list-none;
}

ul a {
    @apply hover:text-gray-400 transition;
}

.menu-button {
    @apply md:hidden text-2xl focus:outline-none;
}

.main-container {
    @apply container mx-auto;
}

.content-wrapper {
    @apply flex flex-col md:flex-row items-center justify-center gap-6 py-10; 
}

.image-container {
    @apply flex justify-center;
}

.image-container img {
    @apply w-2/3 md:w-[350px] lg:w-[450px] rounded-full shadow-lg mx-auto; 
}

.text-container {
    @apply md:w-1/2 text-center md:text-left px-4; 
}

.text-container h1 {
    @apply text-4xl md:text-5xl font-bold text-gray-900;
}

.text-container p {
    @apply mt-3 text-gray-600;
}

.buttons {
    @apply mt-5 flex flex-col md:flex-row gap-3;
}

.btn-blue {
    @apply bg-blue-500 text-white px-4 py-2 rounded hover:bg-blue-600;
}

.btn-green {
    @apply bg-green-500 text-white px-4 py-2 rounded hover:bg-green-600;
}

.card-container {
    @apply container mx-auto grid grid-cols-1 md:grid-cols-3 gap-6 py-8;
}

.card {
    @apply bg-white shadow-lg rounded-lg overflow-hidden;
}

.card img {
    @apply w-full h-48 object-cover;
}

.card-content {
    @apply p-4;
}

.card-content h5 {
    @apply text-lg font-semibold;
}

.card-content p {
    @apply text-gray-600;
}

.swiper-container {
    @apply w-full flex justify-center mt-6; 
}

.mySwiper {
    @apply w-full md:w-4/5 lg:w-3/5; 
}

.swiper-slide {
    @apply flex justify-center items-center;
}

.swiper-slide img {
    @apply w-full h-76 object-cover rounded-lg;
}

.swiper-button-next,
.swiper-button-prev {
    @apply text-white;
}

.footer {
    @apply bg-gray-900 text-white text-center py-4 mt-10;
}

```

Run the command to generate css file

```bash
npx tailwindcss -i ./style.css -o ./dist/output.css
```
It will generate output.css and link it in index.html file

```bash
<head>
    <link rel="stylesheet" href="dist/output.css">
</head>
```

### Output

![Screenshot from 2025-03-30 22-31-07](https://github.com/user-attachments/assets/a528fc47-d947-49fa-861e-03a972b7c1ae)

# Bootstrap 

### Weird way to use Bootstrap

```bash
 <head>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
        <div class="container">
            <a class="navbar-brand" href="#">NASA</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link text-light" href="#">Home</a></li>
                    <li class="nav-item"><a class="nav-link text-light" href="#">About</a></li>
                    <li class="nav-item"><a class="nav-link text-light" href="#">Contact</a></li>
                </ul>
            </div>
        </div>
    </nav>
    
    <div class="container mt-4">
        <div class="row align-items-center">
            <div class="col-md-6 text-center">
                <img style="width: 500px; border-radius: 50%;" src="https://www.nasa.gov/wp-content/themes/nasa/assets/images/default-thumbnail.jpg" class="img-fluid" alt="nasa">
            </div>
            <div class="col-md-6">
                <h1>WELCOME TO NASA</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut harum repudiandae sit eius! Quo animi earum impedit, laudantium quidem fugit ipsa ullam sunt, explicabo veniam non, minus molestiae natus dolorem eum aut rerum rem velit! Illo iusto sapiente, similique quis at dolorum nam eveniet doloremque esse voluptates officiis, maiores vitae?</p>

                <button class="btn btn-info text-light">Explore</button>
                <button class="btn btn-success">Contact</button>
            </div>
        </div>
    </div>

    <div class="container mt-5">
        <div class="row">
            <div class="col-md-4 mb-4">
                <div class="card">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/0e/Venus_Rotation_Movie.gif/640px-Venus_Rotation_Movie.gif" class="card-img-top" alt="Image">
                    <div class="card-body">
                        <h5 class="card-title">Card Title</h5>
                        <p class="card-text">Some description about this card.</p>
                        <button class="btn btn-primary">Learn More</button>
                    </div>
                </div>
            </div>

            <div class="col-md-4 mb-4">
                <div class="card">
                    <img src="https://i.pinimg.com/originals/1a/a2/d5/1aa2d5fee3ea2e2af739959bf3911f3e.gif" class="card-img-top" alt="Image">
                    <div class="card-body">
                        <h5 class="card-title">Card Title</h5>
                        <p class="card-text">Some description about this card.</p>
                        <button class="btn btn-primary">Learn More</button>
                    </div>
                </div>
            </div>
         
                </div>
            </div>
        </div>

        <div id="carouselExampleCaptions" class="carousel slide">
            <div class="carousel-indicators">
              <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
              <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
              <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
            </div>
            <div class="carousel-inner">
              <div class="carousel-item active">
                <img src="https://i.pinimg.com/736x/ab/76/c0/ab76c06b09e4a0812b653ba703e7c557.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-none d-md-block">
                  <h5>First slide label</h5>
                  <p>Some representative placeholder content for the first slide.</p>

                </div>
              </div>
              <div class="carousel-item">
                <img src="https://image.slidesdocs.com/responsive-images/background/blue-beautiful-night-nature-galaxy-space-powerpoint-background_a1cc625475__960_540.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-none d-md-block">
                  <h5>Second slide label</h5>
                  <p>Some representative placeholder content for the second slide.</p>
                </div>
              </div>
              <div class="carousel-item">
                <img src="https://ichef.bbci.co.uk/images/ic/480xn/p023hqw3.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-none d-md-block">
                  <h5>Third slide label</h5>
                  <p>Some representative placeholder content for the third slide.</p>
                </div>
              </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
              <span class="carousel-control-prev-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
              <span class="carousel-control-next-icon" aria-hidden="true"></span>
              <span class="visually-hidden">Next</span>
            </button>
          </div>
    </div>
    <footer class="bg-dark text-white text-center py-3 mt-5">
        <p class="mb-0">© 2024 My Website. All rights reserved.</p>
    </footer>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
```
## Output

![Screenshot from 2025-03-30 22-41-08](https://github.com/user-attachments/assets/fe307012-2012-4068-a542-d6b8f36f451a)

### Professional way to use Tailwindcss

```bash

<head>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="./style.css">
</head>
<body>
    <nav class="nav-bar">
        <div class="nav-container">
            <a class="nav-brand" href="#">NASA</a>
            <button class="nav-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navMenu">
                <span class="nav-toggler-icon"></span>
            </button>
            <div class="nav-collapse" id="navMenu">
                <ul class="nav-list">
                    <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">About</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Contact</a></li>
                </ul>
            </div>
        </div>
    </nav>
    <div class="container">
    <div class="main-container">
        <div class="content-row">
            <div class="image-column">
                <img style="width: 500px; border-radius: 50%;" src="https://www.nasa.gov/wp-content/themes/nasa/assets/images/default-thumbnail.jpg" class="responsive-img" alt="nasa">
            </div>
            <div class="text-column">
                <h1>WELCOME TO NASA</h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut harum repudiandae sit eius! Quo animi earum impedit, laudantium quidem fugit ipsa ullam sunt, explicabo veniam non, minus molestiae natus dolorem eum aut rerum rem velit! Illo iusto sapiente, similique quis at dolorum nam eveniet doloremque esse voluptates officiis, maiores vitae?</p>
                <button class="explore-btn">Explore</button>
                <button class="contact-btn">Contact</button>
            </div>
        </div>
    </div>
    
    <div class="cards-container">
        <div class="cards-row">
            <div class="card-column">
                <div class="card-item">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/0e/Venus_Rotation_Movie.gif/640px-Venus_Rotation_Movie.gif" class="card-image" alt="Venus">
                    <div class="card-content">
                        <h5>Card Title</h5>
                        <p>Some description about this card.</p>
                        <button class="learn-more-btn">Learn More</button>
                    </div>
                </div>
            </div>
           
            <div class="card-column">
                <div class="card-item">
                    <img src="https://i.pinimg.com/originals/1a/a2/d5/1aa2d5fee3ea2e2af739959bf3911f3e.gif" class="card-image" alt="Space">
                    <div class="card-content">
                        <h5>Card Title</h5>
                        <p>Some description about this card.</p>
                        <button class="learn-more-btn">Learn More</button>
                    </div>
                </div>
            </div>
        </div>

        <div class="carousel" id="carouselExampleCaptions">
            <div class="carousel-indicators">
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2" aria-label="Slide 3"></button>
            </div>
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img src="https://i.pinimg.com/736x/ab/76/c0/ab76c06b09e4a0812b653ba703e7c557.jpg" class="carousel-img" alt="Slide 1">
                    <div class="carousel-caption">
                        <h5>First slide label</h5>
                        <p>Some representative placeholder content for the first slide.</p>
                    </div>
                </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Next</span>
            </button>
        </div>
    </div>
</div>
    
    <footer class="footer">
        <p>© 2024 My Website. All rights reserved.</p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
```
style.css

**Use bootstrap classes in style.css directly**

```bash
.nav-bar {
    background-color: var(--bs-dark);
    padding: 1.5rem ;
}

.nav-container {
    max-width: var(--bs-breakpoint-xxl);
    margin-left: auto;
    margin-right: auto;
    padding-left: var(--bs-container-padding-x);
    padding-right: var(--bs-container-padding-x);
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
}

.nav-brand {
    color: var(--bs-light); 
    font-size: var(--bs-navbar-brand-font-size);
    text-decoration: none;
    padding: var(--bs-navbar-brand-padding-y) 0;
    margin-right: var(--bs-navbar-brand-margin-end);
}

.nav-brand:hover {
    color: var(--bs-gray-300);
}

.nav-toggler {
    padding: var(--bs-navbar-toggler-padding-y) var(--bs-navbar-toggler-padding-x);
    background-color: transparent;
    border: var(--bs-navbar-toggler-border-width) solid var(--bs-navbar-dark-toggler-border-color);
    border-radius: var(--bs-navbar-toggler-border-radius);
}

.nav-toggler-icon {
    display: inline-block;
    width: var(--bs-navbar-toggler-icon-width);
    height: var(--bs-navbar-toggler-icon-height);
    background: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'%3e%3cpath stroke='rgba%28255, 255, 255, 0.55%29' stroke-linecap='round' stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/%3e%3c/svg%3e") no-repeat center;
    background-size: 100%;
}

.nav-collapse {
    flex-basis: 100%;
}

.nav-list {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    gap: 8px;
}

.nav-item {
    padding: 0;
}

.nav-link {
    display: block;
    padding: var(--bs-nav-link-padding-y) var(--bs-nav-link-padding-x);
    color: var(--bs-light); 
    text-decoration: none;
    transition: color 0.15s ease-in-out;
}

.nav-link:hover {
    color: var(--bs-gray-300); 
}

@media (min-width: 992px) {
    .nav-collapse {
        flex-basis: auto;
        display: flex !important;
    }
    .nav-list {
        flex-direction: row;
        align-items: center;
        justify-content: flex-end;
    }
}
  .main-container {
    max-width: var(--bs-breakpoint-xxl);
    margin: 1.5rem auto 0; 
    padding-left: var(--bs-container-padding-x);
    padding-right: var(--bs-container-padding-x);
  }
  
  .content-row {
    display: flex;
    flex-wrap: wrap;
    margin-left: calc(var(--bs-gutter-x) * -0.5);
    margin-right: calc(var(--bs-gutter-x) * -0.5);
    align-items: center;
  }
  
  .image-column, .text-column {
    width: 100%;
    padding-left: calc(var(--bs-gutter-x) * 0.5);
    padding-right: calc(var(--bs-gutter-x) * 0.5);
  }
  
  @media (min-width: 768px) {
    .image-column, .text-column {
        width: 50%;
    }
  }
  
  .responsive-img {
    max-width: 100%;
    height: auto;
  }
  
  .text-column h1 {
    font-size: 2.26rem; 
    margin-bottom: 0.5rem;
    color: var(--bs-heading-color);
  }
  
  .text-column p {
    color: var(--bs-body-color);
    margin-left: 20px;
    margin-bottom: 1rem;
  }
  
  .explore-btn {
    background-color: var(--bs-info);
    color: var(--bs-white);
    border: 1px solid var(--bs-info);
    padding: 5px;
    border-radius: 5px;
    margin-right: 0.5rem;
    transition: background-color 0.15s ease-in-out;
  }
  
  .explore-btn:hover {
    background-color: #0ac5e6; 
  }
  
  .contact-btn {
    background-color: var(--bs-success);
    color: var(--bs-white);
    border: 1px solid var(--bs-success);
    padding: 5px;
    border-radius: 5px;
    transition: background-color 0.15s ease-in-out;
  }
  
  .contact-btn:hover {
    background-color: #157347; 
  }
  
  .cards-container {
    max-width: var(--bs-breakpoint-xxl);
    margin: 3rem auto 0; 
    padding-left: var(--bs-container-padding-x);
    padding-right: var(--bs-container-padding-x);
  }
  
  .cards-row {
    display: flex;
    flex-wrap: wrap;
    margin-left: calc(var(--bs-gutter-x) * -0.5);
    margin-right: calc(var(--bs-gutter-x) * -0.5);
  }
  
  .card-column {
    width: 100%;
    padding-left: calc(var(--bs-gutter-x) * 0.5);
    padding-right: calc(var(--bs-gutter-x) * 0.5);
    margin-bottom: 1.5rem; 
  }
  
  @media (min-width: 768px) {
    .card-column {
        width: 33.333%;
    }
  }
  
  .card-item {
    border-radius: 5px;
    background-color: var(--bs-card-bg);
    margin: 2px;
    box-shadow: 0px 6.25px 20px 0px #00000020;
    overflow: hidden;

  }
  
  .card-image {
    width: 100%;
    border-top-left-radius: var(--bs-card-inner-border-radius);
    border-top-right-radius: var(--bs-card-inner-border-radius);
  }
  
  .card-content {
    padding: 5px;
  }
  
  .card-content h5 {
    font-size: 1.25rem; 
    margin-bottom: 0.5rem;
    color: var(--bs-card-title-color);
  }
  
  .card-content p {
    color: var(--bs-card-color);
    margin-bottom: 1rem;
  }
  
  .learn-more-btn {
    background-color: var(--bs-primary);
    color: var(--bs-white);
    border: 1px solid var(--bs-primary);
    padding: 5px;
    border-radius: 5px;
    transition: background-color 0.15s ease-in-out;
  }
  
  .learn-more-btn:hover {
    background-color: #0b5ed7; 
  }
  
  .carousel {
    position: relative;
  }
  
  .carousel-inner {
    position: relative;
    width: 100%;
    overflow: hidden;
  }
  
  .carousel-item {
    display: none;
  }
  
  .carousel-item.active {
    display: block;
  }
  
  .carousel-img {
    width: 100%;
    display: block;
  }
  
  .carousel-caption {
    position: absolute;
    bottom: 1.25rem;
    left: 15%;
    right: 15%;
    color: var(--bs-white);
    text-align: center;
  }
  
  @media (min-width: 768px) {
    .carousel-caption {
        display: block;
    }
  }
  
  .footer {
    background-color: var(--bs-dark);
    color: var(--bs-white);
    text-align: center;
    padding: 1rem 0;
    margin-top: 3rem;
  }
  
  .footer p {
    margin-bottom: 0;
  }
```
## Output

![Screenshot from 2025-03-30 22-46-02](https://github.com/user-attachments/assets/566acee9-b191-41e3-8cab-424c7be448bf)
