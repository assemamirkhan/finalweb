Project Description
 "Flower Shop" is a website dedicated to selling flowers and providing floral services.
 The site offers users a convenient interface to familiarize themselves with products,
 place orders and obtain information about the company.
 Technologies used:
 1. HTML: The main markup language for the site structure.
 2. CSS: Used to style site elements.
 3. JavaScript: The included "script.js" file for interactive elements. The "ScrollReveal"
 library for animations.
 Main functions
 Responsive design:
 ● Navigation menu is optimized for mobile devices.
 ● Product and review grid displays correctly on all screens.
 Interactivity:
 ● Menubutton is activated via JavaScript.
 ● Sections are animated using ScrollReveal.
 Registration form:
 ● Supports field validation via HTML5 (required).
 Folders and files
 1. index.html: Main site file.
 2. style.css: Style file.
 3. script.js: Scripts for interactivity.
Site structure
 1. Navigations
 ● HOME
 ● ABOUT
 ● PRODUCTS
 ● REVIEWS
 ● CONTACTS
 ● Button "SIGN UP".
 Purpose: Provides easy access to the main sections of the site.
 2. Main screen (Header)
 ● Headline with emphasis on keywords ("LET'S EXPLORE UNIQUE
 FLOWERS").
 ● Subheading describing benefits.
 ● "ShopNow" button.
 ● Imageof flowers on the background ("header").
3. About section
 ● Headline: "ABOUT OUR SHOP".
 ● Description of the company's mission.
 ● "Learn More" button to go to additional information.
 4. Section "Our Products"
 Heading: "OUR PRODUCTS". Grid of product cards:
 ● Product image.
 ● Title.
 ● Description.
 ● Price.
 ● "BuyNow"button.
5. Section "Floral Services"
 Grid of cards describing services:
 ● Weddingdecorations.
 ● Corporate gifts.
 ● Custombouquets.
 ● "Learn More" links for each service.
 6. Customer Reviews
 ● Customer photo.
 ● Reviewtext.
 ● Customer name.
7. Registration form (Sign Up)
 ● Full name.
 ● Email.
 ● Password.
 ● "Sign Up" button.
 8. Footer
 ● Companydescription.
 ● Links to social networks.
 ● Quicklinks to the pages "About", "Support", "FAQs", "Terms & Conditions".
 ● Copyright with indication of the owner.
Mainpartsofthecodeandtheirdescription
 1.HTML(index.html)
 <nav>
 <div class="nav__header">
 <div class="nav__logo">
 <a href="#">FLOWER SHOP</a>
 </div>
 <div class="nav__menu__btn" id="menu-btn">
 <i class="ri-menu-line"></i>
 </div>
 </div>
 <ul class="nav__links" id="nav-links">
 <li><a href="#home">HOME</a></li>
 <li><a href="#about">ABOUT</a></li>
 <li><a href="#products">PRODUCTS</a></li>
 <li><a href="#review">REVIEWS</a></li>
 <li><a href="#contacts">CONTACTS</a></li>
 <li>
 <button class="btn"><a href="#sign">SIGN UP</a></button>
 </li>
 </ul>
 </nav>
 Feature:Navigationincludesaresponsivemenuforeaseofuseonmobiledevices.
 <form action="/submit-signup" method="POST" class="signup-form">
 <div class="signup-form__field">
 <label for="name">Full Name</label>
 <input type="text" id="name" name="name" placeholder="Enter your
 full name" required />
 </div>
 <div class="signup-form__field">
 <label for="email">Email Address</label>
 <input type="email" id="email" name="email" placeholder="Enter your
 email address" required />
 </div>
 <div class="signup-form__field">
 <label for="password">Password</label>
 <input type="password" id="password" name="password"
 placeholder="Create a password" required />
 </div>
 <div class="signup-form__field">
 <button type="submit" class="btn">Sign Up</button>
 </div>
 </form>
 Feature:Theformincludesmandatoryfieldswithvalidationviatherequiredattribute.
2.CSS(style.css)
 .btn {
 padding: 0.75rem 1.5rem;
 outline: none;
 border: none;
 font-size: 1rem;
 color: var(--white);
 white-space: nowrap;
 background-color: #ecd0e2;
 border-radius: 5px;
 transition: 0.3s;
 cursor: pointer;
 }
 Feature:Universalstyleforbuttonsusedthroughout thesite.
 3.JavaScript(script.js)
 const menuToggle = document.querySelector('.menu-toggle');
 const navMenu = document.querySelector('.nav-menu');
 menuToggle.addEventListener('click', () => {
 navMenu.classList.toggle('active');
 });
 Feature:Theactiveclassisusedtoshoworhidethemenu(forexample,viaCSSstyles).
 let currentSlide = 0;
 const slides = document.querySelectorAll('.testimonial');
 const nextButton = document.querySelector('.next');
 const prevButton = document.querySelector('.prev');
 function updateSlide() {
 slides.forEach((slide, index) => {
 slide.style.display = index === currentSlide ? 'block' : 'none';
 });
 }
 nextButton.addEventListener('click', () => {
 currentSlide = (currentSlide + 1) % slides.length;
 updateSlide();
 });
 prevButton.addEventListener('click', () => {
 currentSlide = (currentSlide-1 + slides.length) % slides.length;
 updateSlide();
 });
This code implements the testimonial slider:
 Slides: Stored in the slides variable, the current slide is tracked via currentSlide.
 Toggle: The nextButton and prevButton buttons toggle slides forward and backward.
 Update: The updateSlide function hides all slides except the current one using display.
 Carousel: The indexes are cycled using modular arithmetic.
 CONCLUSION:
 The "Flower Shop" project successfully delivers a responsive and interactive website
 for floral services. With modern technologies like HTML, CSS, and JavaScript, it
 ensures a user-friendly experience through a mobile-optimized design, interactive
 features, and secure registration forms. Key sections like "Our Products" and
 "Customer Reviews" enhance engagement, while smooth animations add a polished
 touch. This project sets a strong foundation for future enhancements, showcasing a
 professional and customer-focused design
