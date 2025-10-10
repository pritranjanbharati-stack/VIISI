<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Visiontech Communication</title>
    <!-- Removed external CSS link and included essential styles here -->
    <style>
        /* General Setup */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        /* Utility classes */
        .container { max-width: 1200px; margin: 0 auto; padding: 0 15px; }

        /* Offer Bar */
        .offer-bar {
            background-color: #ffcc00;
            color: #333;
            padding: 5px 0;
            text-align: center;
            font-size: 14px;
        }
        .offer-bar marquee { display: block; }

        /* Header */
        .header {
            background-color: #fff;
            padding: 10px 0;
            border-bottom: 1px solid #ddd;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }
        .logo img { height: 60px; width: auto; cursor: pointer; padding: 0 15px; }

        /* Search Bar */
        .search-bar {
            display: flex;
            flex-grow: 1;
            max-width: 600px;
            margin: 10px 15px;
            border: 2px solid #007bff;
            border-radius: 8px;
            overflow: hidden;
        }
        .search-bar select, .search-bar input[type="text"] {
            padding: 10px;
            border: none;
            outline: none;
            font-size: 16px;
            background-color: #f9f9f9;
        }
        .search-bar select { border-right: 1px solid #ddd; cursor: pointer; }
        .search-bar input[type="text"] { flex-grow: 1; }
        .search-bar button {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 10px 15px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s;
        }
        .search-bar button:hover { background-color: #0056b3; }

        /* Header Links */
        .header-links { display: flex; gap: 20px; padding: 0 15px; }
        .header-links a {
            text-decoration: none;
            color: #007bff;
            font-weight: bold;
            transition: color 0.3s;
        }
        .header-links a:hover { color: #0056b3; }

        /* Nav Menu */
        nav {
            background-color: #333;
            padding: 10px 0;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        nav a {
            color: white;
            text-decoration: none;
            padding: 8px 15px;
            font-size: 15px;
            transition: background-color 0.3s;
        }
        nav a:hover { background-color: #007bff; }
        
        /* ====== Slider ====== */
.slider-container {
  position: relative;
  width: 100%;
  height: 70vh;
  margin: 0;
  overflow: hidden;
}
.slides {
  display: flex;
  width: 100%;
  height: 100%;
  transition: transform 0.5s ease-in-out;
}
.slides img {
  width: 100%;
  flex-shrink: 0;
  object-fit: cover;
}
.prev, .next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: rgba(0,0,0,0.5);
  color: #fff;
  padding: 10px;
  border: none;
  cursor: pointer;
  border-radius: 50%;
  z-index: 10;
}
.prev { left: 20px; }
.next { right: 20px; }
.dots {
  text-align: center;
  margin-top: 10px;
}
.dot {
  display: inline-block;
  height: 12px;
  width: 12px;
  margin: 5px;
  background: #bbb;
  border-radius: 50%;
  cursor: pointer;
}
.active { background: #333; }

/* ===== Global Styles ===== */
body {
  font-family: "Segoe UI", Arial, sans-serif;
  margin: 0;
  padding: 0;
  background: #f9f9f9;
  color: #333;
}
.section-title {
  text-align: center;
  font-size: 2.2rem;
  margin: 50px 0 30px;
  color: #004080;
  position: relative;
  animation: fadeDown 1s ease-in-out;
}

        /* Services & Products Sections */
        section { padding: 40px 15px; text-align: center; }
        .section-title { font-size: 2em; margin-bottom: 20px; color: #007bff; }

        .services-grid, .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        .service-card, .product-card {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            text-align: center;
        }
        .service-icon { font-size: 2.5em; color: #007bff; margin-bottom: 10px; }
        .service-card h3, .product-card h4 { margin-top: 0; color: #333; }
        
        .product-card { text-align: left; }
        .product-image { width: 100%; height: 200px; object-fit: cover; border-radius: 4px; margin-bottom: 10px; }
        .product-content h4 { font-size: 1.2em; margin-bottom: 5px; }
        .product-content p { font-size: 0.9em; color: #666; }

        /* Footer */
        footer { background-color: #222; color: #fff; padding: 30px 0 10px; }
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        .footer-col h4 { border-bottom: 2px solid #007bff; padding-bottom: 10px; margin-bottom: 15px; }
        .footer-col ul { list-style: none; padding: 0; }
        .footer-col ul li a { color: #ccc; text-decoration: none; display: block; margin-bottom: 8px; transition: color 0.3s; }
        .footer-col ul li a:hover { color: #007bff; }
        .contact-info p, .contact-info h4 { margin: 5px 0; font-size: 0.9em; }
        
        .newsletter input { padding: 8px; width: calc(100% - 100px); border: none; border-radius: 4px 0 0 4px; }
        .newsletter button { padding: 8px 15px; background-color: #007bff; color: white; border: none; border-radius: 0 4px 4px 0; cursor: pointer; transition: background-color 0.3s; }
        .newsletter button:hover { background-color: #0056b3; }
        
        .footer-bottom { text-align: center; padding-top: 20px; border-top: 1px solid #444; margin-top: 20px; }

        /* Modals and Forms Styling */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.7);
            display: none; /* Initially hidden */
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }
        .modal-content {
            background: white;
            padding: 30px;
            border-radius: 10px;
            width: 90%;
            max-width: 500px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            position: relative;
            max-height: 90vh;
            overflow-y: auto;
        }
        .modal-content h2 { color: #007bff; margin-top: 0; border-bottom: 2px solid #ddd; padding-bottom: 10px; margin-bottom: 20px; }
        .modal-content label { display: block; margin-bottom: 5px; font-weight: bold; }
        .modal-content input[type="text"], 
        .modal-content input[type="email"], 
        .modal-content input[type="password"] {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 5px;
            box-sizing: border-box;
        }
        .modal-content button.close-btn {
            position: absolute;
            top: 10px;
            right: 10px;
            background: none;
            border: none;
            font-size: 24px;
            cursor: pointer;
            color: #333;
        }
        .modal-content button.submit-btn {
            background-color: #007bff;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            width: 100%;
            transition: background-color 0.3s;
        }
        .modal-content button.submit-btn:hover { background-color: #0056b3; }

        /* Custom Message Box */
        #custom-message {
            position: fixed; 
            top: 20px; 
            right: 20px; 
            background: #4CAF50; 
            color: white; 
            padding: 15px; 
            border-radius: 8px; 
            z-index: 1001; 
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1); 
            transition: opacity 0.3s;
            display: none;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header { flex-direction: column; align-items: flex-start; }
            .logo { margin-bottom: 10px; }
            .search-bar { width: 100%; max-width: 100%; margin: 10px 0; }
            .header-links { width: 100%; justify-content: space-around; padding: 10px 0; border-top: 1px solid #eee; }
            nav a { padding: 8px 10px; font-size: 14px; }
        }
    </style>
    <!-- Font Awesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
</head>
<body>

<!-- Custom Message Box -->
<div id="custom-message"></div>

<!-- Offer Bar -->
<div class="offer-bar">
    <marquee>On Every Purchase Get Flat ₹100 Discounts. | USE CODE : <b>FIRSTTIME</b></marquee>
</div>

<!-- Header -->
<div class="header container">
    <div class="logo">
        <img src="https://cdn.dotpe.in/longtail/store-logo/9099859/HQOvszBT.webp" 
            alt="Visiontech Communication" 
            style="height:60px; width:auto; cursor:pointer;">
    </div>


    <div class="search-bar">
        <select>
            <option>All Category</option>
            <option>Laptops</option>
            <option>Printers & Scanner</option>
            <option>Monitors</option>
        </select>
        <input type="text" placeholder="Search Products">
        <button>🔍</button>
    </div>

    <div class="header-links">
        <!-- Links updated to use JavaScript functions to open modals -->
        <a href="#" onclick="openModal('about-us-modal')">About Us</a>
        <a href="#" onclick="openModal('login-modal')">Login</a>
        <a href="#" onclick="openModal('register-modal')">Register</a>
    </div>
</div>
<!-- Nav Menu -->
<nav>
    <a href="#">All Category</a>
    <a href="#">Laptops</a>
    <a href="#">Printers & Scanner</a>
    <a href="#">Monitors</a>
    <a href="#">Accessories & Peripherals</a>
    <a href="#">Audio Accessories</a>
    <a href="#">Build Own PC</a>
    <a href="#">Support</a>
    <a href="#">Offer Zone</a>
</nav>

<!-- Slider -->
<div class="slider-container">
    <div class="slides">
        <img src="https://img.freepik.com/free-vector/flat-design-electronics-store-facebook-cover_23-2151098080.jpg">
        <img src="https://www.shutterstock.com/image-vector/electron…ional-shopping-sale-computer-260nw-1190458762.jpg">
        <img src="https://www.shutterstock.com/image-vector/online-e…ics-shopping-delivery-banner-260nw-2282200763.jpg">
    </div>

    <!-- Buttons -->
    <button class="prev">&#10094;</button>
    <button class="next">&#10095;</button>
</div>

<!-- Dots -->
<div class="dots">
    <span class="dot active"></span>
    <span class="dot"></span>
    <span class="dot"></span>
</div>

<section id="services" class="container">
    <h2 class="section-title">Our Services</h2>
    <div class="services-grid">
        <div class="service-card">
            <div class="service-icon"><i class="fas fa-phone-volume"></i></div>
            <h3>Telecommunication Solutions</h3>
            <p>Providing advanced telecommunication infrastructure and support for seamless connectivity.</p>
        </div>
        <div class="service-card">
            <div class="service-icon"><i class="fas fa-network-wired"></i></div>
            <h3>Network Installation & Maintenance</h3>
            <p>Expert network setup and ongoing maintenance to ensure optimal performance.</p>
        </div>
        <div class="service-card">
            <div class="service-icon"><i class="fas fa-cloud"></i></div>
            <h3>Cloud Communication</h3>
            <p>Cloud-based communication platforms to enhance collaboration and productivity.</p>
        </div>
        <div class="service-card">
            <div class="service-icon"><i class="fas fa-headset"></i></div>
            <h3>Consulting & Support</h3>
            <p>Professional consulting services to tailor communication strategies to your needs.</p>
        </div>
    </div>
</section>

<section id="products" class="container">
    <h2 class="section-title">Our Products</h2>
    <div class="products-grid">
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1519389950473-47ba0277781c?auto=format&fit=crop&w=600&q=80" alt="Product 1" class="product-image" />
            <div class="product-content">
                <h4>VisionTech Router X100</h4>
                <p>High-speed router designed for enterprise-grade connectivity and security.</p>
            </div>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1504384308090-c894fdcc538d?auto=format&fit=crop&w=600&q=80" alt="Product 2" class="product-image" />
            <div class="product-content">
                <h4>CloudComm Platform</h4>
                <p>Scalable cloud communication platform for unified messaging and collaboration.</p>
            </div>
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=600&q=80" alt="Product 3" class="product-image" />
            <div class="product-content">
                <h4>SecureNet Firewall</h4>
                <p>Advanced firewall solution to protect your network from cyber threats.</p>
            </div> 
        </div>
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=600&q=80" alt="Product 3" class="product-image" />
            <div class="product-content">
                <h4>SecureNet Firewall</h4>
                <p>Advanced firewall solution to protect your network from cyber threats.</p>
            </div>
        </div>
    </div>
</section>

<!-- Footer Section -->
<footer>
    <div class="footer-container">

        <!-- Information -->
        <div class="footer-col">
            <h4>Information</h4>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About Us</a></li>
                <li><a href="#">Categories</a></li>
                <li><a href="#">Store</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Contact Us</a></li>
                <li><a href="#">FAQ</a></li>
                <li><a href="#">Sitemap</a></li>
                <li><a href="#">Support</a></li>
                <li><a href="#">Our Client</a></li>
                <li><a href="#">Our Partner</a></li>
                <li><a href="#">Warranty</a></li>
                <li><a href="#">Software Driver</a></li>
                <li><a href="#">Offer Zone</a></li>
            </ul>
        </div>

        <!-- Our Category -->
        <div class="footer-col">
            <h4>Our Category</h4>
            <ul>
                <li><a href="#">Laptops</a></li>
                <li><a href="#">Printers & Scanner</a></li>
                <li><a href="#">Monitors</a></li>
                <li><a href="#">Accessories & Peripherals</a></li>
                <li><a href="#">Audio Accessories</a></li>
                <li><a href="#">Network Device</a></li>
                <li><a href="#">Build Own PC</a></li>
                <li><a href="#">Gaming Device</a></li>
                <li><a href="#">Smart Device</a></li>
                <li><a href="#">Security Camera</a></li>
                <li><a href="#">Open Box Product</a></li>
                <li><a href="#">Cables & Power Adapters</a></li>
                <li><a href="#">View All</a></li>
            </ul>
        </div>

        <!-- Policies -->
        <div class="footer-col">
            <h4>Policies</h4>
            <ul>
                <li><a href="#">Shipping Policy</a></li>
                <li><a href="#">Refund & Return Policy</a></li>
                <li><a href="#">Terms & Conditions</a></li>
                <li><a href="#">Privacy Policy</a></li>
                <li><a href="#">Warranty</a></li>
                <li><a href="#">Software Driver</a></li>
                <li><a href="#">Offer Zone</a></li>
            </ul>
                <!-- My Account -->
        <div class="footer-col">
            <h4>My Account</h4>
            <ul>
                <li><a href="#">My Profile</a></li>
                <li><a href="#">My Orders</a></li>
                <li><a href="#">Return & Refund</a></li>
                <li><a href="#">Raise Ticket</a></li>
                <li><a href="#">Support</a></li>
            </ul>
        </div>
        </div>



        <!-- Contact -->
        <div class="footer-col">
            <h4>Contact Us</h4>
            <div class="contact-info">
                <p>B07, H-140, Secter 63 Noida, Uttare Pradesh, India</p>
                <p>📞 +91-9818346141, 9205864623</p>
                <p>📧 sales@Visiontechcommunication.in</p>
                <p>📧 Visiontech2930@gmail.com</p>
                <h4>Subscribe</h4>
                <div class="footer-col newsletter"></div>
            <input type="email" id="email" placeholder="Enter your email..." />
            <button onclick="subscribe()">Subscribe</button>
            </div>
            </div>
        </div>
    </div>
            <!-- Footer Bottom -->
    <div class="footer-bottom">
        <p>Copyright © <span id="year"></span> Visiontech Communication. All rights reserved.</p>
    </div>
</footer>


<!-- ============================================== -->
<!-- MODALS/FORMS SECTION -->
<!-- ============================================== -->

<!-- 1. Login Modal -->
<div id="login-modal" class="modal-overlay" onclick="closeModalOnOutsideClick(event)">
    <div class="modal-content">
        <button class="close-btn" onclick="closeModal('login-modal')">&times;</button>
        <h2>Login to Your Account</h2>
        <form onsubmit="handleFormSubmit(event, 'Login')">
            <label for="login-email">Email Address</label>
            <input type="email" id="login-email" required placeholder="Enter your email" />

            <label for="login-password">Password</label>
            <input type="password" id="login-password" required placeholder="Enter your password" />

            <button type="submit" class="submit-btn">Login</button>
            <p style="text-align: center; margin-top: 15px;">Don't have an account? <a href="#" onclick="showRegisterFromLogin()">Register here</a></p>
        </form>
    </div>
</div>

<!-- 2. Register Modal -->
<div id="register-modal" class="modal-overlay" onclick="closeModalOnOutsideClick(event)">
    <div class="modal-content">
        <button class="close-btn" onclick="closeModal('register-modal')">&times;</button>
        <h2>Create New Account</h2>
        <form onsubmit="handleFormSubmit(event, 'Register')">
            <label for="reg-name">Full Name</label>
            <input type="text" id="reg-name" required placeholder="Enter your name" />
            
            <label for="reg-email">Email Address</label>
            <input type="email" id="reg-email" required placeholder="Enter your email" />

            <label for="reg-password">Password</label>
            <input type="password" id="reg-password" required placeholder="Choose a secure password" />

            <button type="submit" class="submit-btn">Register</button>
            <p style="text-align: center; margin-top: 15px;">Already have an account? <a href="#" onclick="showLoginFromRegister()">Login here</a></p>
        </form>
    </div>
</div>

<!-- 3. About Us Modal -->
<div id="about-us-modal" class="modal-overlay" onclick="closeModalOnOutsideClick(event)">
    <div class="modal-content">
        <button class="close-btn" onclick="closeModal('about-us-modal')">&times;</button>
        <h2>About Visiontech Communication</h2>
        <p style="margin-bottom: 15px;">Visiontech Communication is a leading provider of high-quality IT products and comprehensive telecommunication solutions. Our mission is to empower businesses and individuals with cutting-edge technology and unparalleled support.</p>
        
        <h3 style="font-size: 1.2em; margin-top: 20px; color: #333;">Our Values:</h3>
        <ul style="list-style-type: disc; margin-left: 20px; font-size: 0.9em;">
            <li>Innovation and Quality in every product.</li>
            <li>Commitment to Customer Success.</li>
            <li>Integrity and Trust in all our dealings.</li>
        </ul>
        
        <h3 style="font-size: 1.2em; margin-top: 20px; color: #333;">Contact Information:</h3>
        <p style="font-size: 0.9em;">
            Location: B07, H-140, Secter 63 Noida, Uttare Pradesh, India<br>
            Phone: +91-9818346141<br>
            Email: sales@Visiontechcommunication.in
        </p>
    </div>
</div>

<!-- ============================================== -->
<!-- JAVASCRIPT -->
<!-- ============================================== -->
<script>
    // Slider Logic
    const slides = document.querySelector('.slides');
    const images = document.querySelectorAll('.slides img');
    const prev = document.querySelector('.prev');
    const next = document.querySelector('.next');
    const dots = document.querySelectorAll('.dot');

    let index = 0;

    function showSlide(i) {
        index = (i + images.length) % images.length;
        slides.style.transform = `translateX(${-index * 100}%)`;
        dots.forEach(dot => dot.classList.remove('active'));
        dots[index].classList.add('active');
    }

    next.addEventListener('click', () => showSlide(index + 1));
    prev.addEventListener('click', () => showSlide(index - 1));

    dots.forEach((dot, i) => {
        dot.addEventListener('click', () => showSlide(i));
    });

    // Auto slide
    setInterval(() => showSlide(index + 1), 4000);

    // Auto update year for footer
    document.getElementById("year").textContent = new Date().getFullYear();

    // Custom Message Display Function (Replaces alert())
    function showMessage(text, isSuccess) {
        const messageContainer = document.getElementById('custom-message');
        const bgColor = isSuccess ? '#4CAF50' : '#f44336'; 
        
        messageContainer.style.background = bgColor;
        messageContainer.textContent = text;
        messageContainer.style.display = 'block';
        messageContainer.style.opacity = '1';
        
        // Hide message after 3 seconds
        setTimeout(() => {
            messageContainer.style.opacity = '0';
            setTimeout(() => {
                 messageContainer.style.display = 'none';
            }, 300);
        }, 3000);
    }

    // Newsletter subscription logic
    function subscribe() {
        const emailInput = document.getElementById("email");
        const email = emailInput.value;
        
        if (email && email.includes('@') && email.includes('.')) {
            showMessage("Thank you for subscribing: " + email, true);
            emailInput.value = "";
        } else {
            showMessage("Please enter a valid email address.", false);
        }
    }

    // Modal Functions
    function openModal(modalId) {
        document.getElementById(modalId).style.display = 'flex';
    }

    function closeModal(modalId) {
        document.getElementById(modalId).style.display = 'none';
    }

    function closeModalOnOutsideClick(event) {
        if (event.target.classList.contains('modal-overlay')) {
            event.target.style.display = 'none';
        }
    }

    // Form Submission Handler (Prevents page reload and shows message)
    function handleFormSubmit(event, formName) {
        event.preventDefault();
        
        // In a real application, you would send data to a server here.
        showMessage(`${formName} successful! (Demo) - Data not saved.`, true);

        // Optionally close the modal after submission
        if (formName === 'Login') {
            closeModal('login-modal');
        } else if (formName === 'Register') {
            closeModal('register-modal');
        }

        // Clear the form fields
        event.target.reset();
    }
    
    // Switch between Login and Register Modals
    function showRegisterFromLogin() {
        closeModal('login-modal');
        openModal('register-modal');
    }

    function showLoginFromRegister() {
        closeModal('register-modal');
        openModal('login-modal');
    }
</script>

</body>
</html>
