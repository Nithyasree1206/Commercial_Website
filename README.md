# Ex02 Commercial Website
## Date:07.05.2026
## Name: NITHYASREE S
## Reg No: 212224040225

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
## index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gloria Jewellery - Premium Jewelry Collection</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">
                <img src="logo.png" alt="Gloria Jewellery Logo">
                <span>Gloria Jewellery</span>
            </div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="hamburger">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </nav>
    </header>

    <main>
        <section id="home" class="hero">
            <div class="hero-content">
                <h1>Welcome to Gloria Jewellery</h1>
                <p>Discover exquisite jewelry pieces that sparkle with elegance</p>
                <a href="#products" class="cta-button">Explore Collection</a>
            </div>
        </section>

        <section id="products" class="products">
            <h2>Our Jewelry Collection</h2>
            <div class="product-grid">
                <div class="product-card">
                    <div class="product-image">
                        <img src="https://images.unsplash.com/photo-1515562141207-7a88fb7ce338?ixlib=rb-4.0.3&auto=format&fit=crop&w=687&q=80" alt="Diamond Necklace">
                    </div>
                    <h3>Diamond Necklace</h3>
                    <p>Elegant diamond necklace for special occasions</p>
                    <span class="price">$299.99</span>
                    <button class="buy-button">Add to Cart</button>
                </div>
                <div class="product-card">
                    <div class="product-image">
                        <img src="https://images.unsplash.com/photo-1535632066927-ab7c9ab60908?ixlib=rb-4.0.3&auto=format&fit=crop&w=687&q=80" alt="Gold Earrings">
                    </div>
                    <h3>Gold Earrings</h3>
                    <p>Stunning gold earrings with intricate design</p>
                    <span class="price">$149.99</span>
                    <button class="buy-button">Add to Cart</button>
                </div>
                <div class="product-card">
                    <div class="product-image">
                        <img src="https://images.unsplash.com/photo-1602173574767-37ac01994b2a?ixlib=rb-4.0.3&auto=format&fit=crop&w=687&q=80" alt="Silver Bracelet">
                    </div>
                    <h3>Silver Bracelet</h3>
                    <p>Classic silver bracelet for everyday elegance</p>
                    <span class="price">$79.99</span>
                    <button class="buy-button">Add to Cart</button>
                </div>
                <div class="product-card">
                    <div class="product-image">
                        <img src="https://images.unsplash.com/photo-1605100804763-247f67b3557e?ixlib=rb-4.0.3&auto=format&fit=crop&w=687&q=80" alt="Pearl Ring">
                    </div>
                    <h3>Pearl Ring</h3>
                    <p>Timeless pearl ring with gold band</p>
                    <span class="price">$199.99</span>
                    <button class="buy-button">Add to Cart</button>
                </div>
            </div>
        </section>

        <section id="about" class="about">
            <div class="about-content">
                <h2>About Gloria Jewellery</h2>
                <p>We are passionate about crafting and curating the finest jewelry pieces. Each item in our collection is carefully selected to ensure it meets our standards of quality, craftsmanship, and timeless beauty.</p>
            </div>
        </section>
    </main>

    <footer>
        <div class="footer-content">
            <div class="footer-section">
                <h3>Gloria Jewellery</h3>
                <p>Your destination for exquisite jewelry</p>
            </div>
            <div class="footer-section">
                <h3>Quick Links</h3>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#products">Products</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </div>
            <div class="footer-section">
                <h3>Contact Us</h3>
                <p>Email: info@gloriajewellery.com</p>
                <p>Phone: +91 98765 43210</p>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2026 Gloria Jewellery. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
```
## style.css
```
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}
body{
  font-family:Arial,sans-serif;
  color:#333;
}
/* HEADER */
header{
  background:rgba(0,0,0,0.5);
  position:fixed;
  width:100%;
}
nav{
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:15px 40px;
}
.logo{
  display:flex;
  align-items:center;
  gap:10px;
  color:gold;
  font-size:18px;
  font-weight:bold;
}

.logo img{
  height:50px;
  width:50px;
  object-fit:contain;
  display:block;
}
.nav-links{
  display:flex;
  list-style:none;
  gap:20px;
}
.nav-links a{
  color:white;
  text-decoration:none;
}
.nav-links a:hover{
  color:gold;
}
/* HERO */
.hero{
  height:100vh;
  background:
  linear-gradient(rgba(0,0,0,0.5),rgba(0,0,0,0.5)),
  url('https://images.unsplash.com/photo-1515562141207-7a88fb7ce338');
  background-size:cover;
  background-position:center;
  display:flex;
  justify-content:center;
  align-items:center;
  text-align:center;
  color:white;
}
.hero h1{
  font-size:50px;
}
.hero p{
  margin:15px 0;
}
.cta-button{
  background:gold;
  color:black;
  padding:10px 20px;
  text-decoration:none;
  border-radius:5px;
}
/* PRODUCTS */
.products{
  padding:70px 20px;
  background:#f5f5f5;
}
.products h2{
  text-align:center;
  margin-bottom:30px;
}
.product-grid{
  display:flex;
  justify-content:center;
  gap:20px;
  flex-wrap:wrap;
}
.product-card{
  width:250px;
  background:white;
  border-radius:10px;
  overflow:hidden;
  text-align:center;
  box-shadow:0 0 10px rgba(0,0,0,0.2);
}
.product-card img{
  width:100%;
  height:250px;
  object-fit:cover;
}
.price{
  color:goldenrod;
  font-weight:bold;
}
.buy-button{
  margin:15px;
  padding:10px 20px;
  border:none;
  background:black;
  color:white;
}
/* ABOUT */
.about{
  padding:60px 20px;
  text-align:center;
}
/* FOOTER */
footer{
  background:#111;
  color:white;
  padding:40px 20px;
}
.footer-content{
  display:flex;
  justify-content:space-around;
  flex-wrap:wrap;
  gap:20px;
}
.footer-section{
  text-align:center;
}
.footer-logo,
.footer-section h3{
  color:gold;
}
.footer-section a{
  display:block;
  color:#ddd;
  text-decoration:none;
  margin:5px 0;
}
.footer-bottom{
  text-align:center;
  margin-top:20px;
  border-top:1px solid #444;
  padding-top:15px;
}
/* RESPONSIVE */
@media(max-width:768px){
  nav,
  .footer-content{
    flex-direction:column;
    text-align:center;
  }

  .nav-links{
    flex-direction:column;
  }
}
```
## OUTPUT
<img width="1886" height="906" alt="image" src="https://github.com/user-attachments/assets/c6b13fee-e769-4747-9565-578912d798d3" />
<img width="1890" height="917" alt="image" src="https://github.com/user-attachments/assets/2b3fd53b-7aee-4a54-ab30-bc140dc13396" />
<img width="1887" height="897" alt="image" src="https://github.com/user-attachments/assets/2bc74ccf-ff80-48cd-9224-dd34eaf4af21" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
