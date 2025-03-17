# TRUE-NORTH
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>True North Geospatials Ltd</title>
  <style>
    body {
      font-family: 'Georgia', serif; /* Default font for body text */
      line-height: 1.6;
      margin: 0;
      padding: 0;
      background-color: #f5f5dc; /* Beige background */
      color: #333;
    }
    .banner {
      width: 100%;
      height: 300px; /* Adjust height as needed */
      background-image: url('WhatsApp_Image_2025-03-17_at_12.55.40.jpeg'); /* New image */
      background-size: cover; /* Crop and fit the image */
      background-position: center; /* Center the image */
      position: relative; /* For overlay positioning */
      display: flex; /* Flexbox for centering */
      justify-content: center; /* Center horizontally */
      align-items: center; /* Center vertically */
    }
    .banner::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.4); /* Semi-transparent black overlay */
    }
    header {
      text-align: center;
      color: #fff;
      position: relative; /* Ensure text is above the overlay */
      z-index: 1; /* Bring text to the front */
    }
    header h1 {
      margin: 0;
      font-size: 2.5rem;
      font-family: 'Montserrat', sans-serif; /* Modern font for headings */
      font-weight: 700; /* Bold for emphasis */
    }
    header p {
      margin: 10px 0 0;
      font-size: 1.2rem;
      font-family: 'Raleway', sans-serif; /* Elegant font for tagline */
      font-weight: 300; /* Light for contrast */
    }
    nav {
      background: #6B5B4D; /* Darker brown for contrast */
      color: #fff;
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: #fff;
      margin: 0 15px;
      text-decoration: none;
      font-family: 'Montserrat', sans-serif; /* Consistent font for navigation */
    }
    .container {
      width: 80%;
      margin: 20px auto;
      background: #fff;
      padding: 20px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      border-radius: 8px;
    }
    h2 {
      color: #8B7355; /* Beige-complementary dark brown */
      font-family: 'Montserrat', sans-serif; /* Modern font for headings */
      font-weight: 600; /* Semi-bold for emphasis */
    }
    ul {
      list-style-type: disc; /* Add bullets to lists */
      padding-left: 20px; /* Indent bullets */
    }
    ul li {
      margin-bottom: 10px;
    }
    .services-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr); /* Two columns */
      gap: 20px; /* Space between boxes */
    }
    .service-box {
      border: 3px solid #8B7355; /* Dark brown border */
      padding: 20px;
      border-radius: 8px;
      opacity: 0; /* Initially hidden */
      transform: translateX(-100%); /* Start off-screen */
      transition: opacity 1s ease, transform 1s ease;
    }
    .service-box.visible {
      opacity: 1;
      transform: translateX(0);
    }
    .service-box strong {
      font-family: 'Montserrat', sans-serif; /* Modern font for service titles */
      font-weight: 600; /* Semi-bold for emphasis */
    }
    .service-box ul {
      font-family: 'Raleway', sans-serif; /* Elegant font for service details */
      font-weight: 400; /* Regular weight for readability */
    }
    .feedback-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr); /* Two columns */
      gap: 20px; /* Space between boxes */
      margin-top: 20px;
    }
    .feedback-box {
      border: 3px solid #8B7355; /* Dark brown border */
      padding: 20px;
      border-radius: 8px;
      opacity: 0; /* Initially hidden */
      transform: translateY(50px); /* Start slightly below */
      transition: opacity 1s ease, transform 1s ease;
    }
    .feedback-box.visible {
      opacity: 1;
      transform: translateY(0);
    }
    .feedback-box p {
      font-family: 'Raleway', sans-serif;
      font-style: italic;
      color: #555;
    }
    footer {
      background: #6B5B4D; /* Darker brown for contrast */
      color: #fff;
      text-align: center;
      padding: 10px 0;
      margin-top: 20px;
    }
    .map {
      width: 100%;
      height: 300px;
      border: 0;
      border-radius: 8px;
      margin-top: 20px;
    }

    /* Centered Drone Mapping & LiDAR Surveys box */
    .drone-box {
      grid-column: 1 / -1; /* Span full width */
      max-width: 600px; /* Limit width for better readability */
      margin: 0 auto; /* Center horizontally */
    }

    /* Contact Us Icons */
    .contact-info {
      display: flex;
      flex-direction: column;
      gap: 15px; /* Space between items */
    }
    .contact-item {
      display: flex;
      align-items: center;
      gap: 10px; /* Space between icon and text */
    }
    .contact-item i {
      font-size: 1.5rem; /* Icon size */
      color: #8B7355; /* Dark brown color */
    }
    .contact-item p {
      margin: 0;
      font-family: 'Raleway', sans-serif;
      font-size: 1rem;
      color: #333;
    }
  </style>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Raleway:wght@300;400&display=swap" rel="stylesheet">
  <!-- Font Awesome Icons -->
  <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
</head>
<body>
  <!-- Banner Image at the Beginning -->
  <div class="banner">
    <header>
      <h1>True North Geospatials Ltd</h1>
      <p>Navigating land. Defining space.</p>
    </header>
  </div>

  <nav>
    <a href="#about">About Us</a>
    <a href="#services">Our Services</a>
    <a href="#feedback">Feedback</a>
    <a href="#contact">Contact Us</a>
  </nav>

  <div class="container">
    <section id="about">
      <h2>About Us</h2>
      <p>
        True North Geospatials Ltd is a professional land survey and geospatial consultancy firm based in Kiambu, Kenya. We specialize in sectional property surveys, ensuring accuracy, compliance, and efficiency in land subdivision and registration. Our expertise extends to geospatial data analysis, mapping, and remote sensing, providing clients with reliable land solutions.
      </p>
    </section>

    <section id="services">
      <h2>Our Services</h2>
      <div class="services-grid">
        <div class="service-box">
          <strong>Sectional Property Surveys</strong>
          <ul>
            <li>Preparation of Sectional Plans in compliance with the Sectional Properties Act, 2020.</li>
            <li>Beacon re-establishment and re-survey of existing sectional developments.</li>
            <li>Spatial documentation for multi-unit developments to facilitate property registration.</li>
          </ul>
        </div>
        <div class="service-box">
          <strong>Land & Cadastral Surveys</strong>
          <ul>
            <li>Boundary identification and re-establishment to resolve disputes.</li>
            <li>Processing mutation surveys for land subdivision or amalgamation.</li>
            <li>Title deed verification and due diligence for land transactions.</li>
          </ul>
        </div>
        <div class="service-box">
          <strong>Geospatial Mapping & GIS Solutions</strong>
          <ul>
            <li>Topographic surveys and digital mapping for infrastructure planning.</li>
            <li>GIS database creation and analysis for land use planning.</li>
            <li>Remote sensing and drone mapping for high-accuracy spatial data.</li>
          </ul>
        </div>
        <div class="service-box">
          <strong>Engineering & Construction Surveys</strong>
          <ul>
            <li>Setting out surveys for roads, buildings, and infrastructure projects.</li>
            <li>As-built surveys for project documentation and compliance.</li>
            <li>Elevation and contour mapping for design and construction purposes.</li>
          </ul>
        </div>
        <div class="service-box drone-box"> <!-- Centered Drone Mapping & LiDAR Surveys box -->
          <strong>Drone Mapping & LiDAR Surveys</strong>
          <ul>
            <li>Aerial surveys for large-scale mapping and terrain modeling.</li>
            <li>LiDAR-based 3D modeling for detailed site analysis.</li>
            <li>Flood and drainage analysis using high-resolution elevation data.</li>
          </ul>
        </div>
      </div>
    </section>

    <section id="feedback">
      <h2>What Our Clients Say</h2>
      <div class="feedback-grid">
        <div class="feedback-box">
          <p><strong>John K.</strong> (Nairobi): "True North Geospatials provided accurate and timely survey services for our property. Highly recommended!"</p>
        </div>
        <div class="feedback-box">
          <p><strong>Mary W.</strong> (Kiambu): "Their team is professional and knowledgeable. They made the entire process seamless."</p>
        </div>
        <div class="feedback-box">
          <p><strong>Peter M.</strong> (Mombasa): "The drone mapping services were top-notch. We got detailed and precise data for our project."</p>
        </div>
        <div class="feedback-box">
          <p><strong>Grace N.</strong> (Nakuru): "Excellent customer service and attention to detail. Will definitely work with them again."</p>
        </div>
      </div>
    </section>

    <section id="contact">
      <h2>Contact Us</h2>
      <div class="contact-info">
        <div class="contact-item">
          <i class="fas fa-map-marker-alt"></i> <!-- Location Icon -->
          <p>Kiambu, Kenya</p>
        </div>
        <div class="contact-item">
          <i class="fas fa-phone"></i> <!-- Phone Icon -->
          <p>+254727811576 / +254738640372</p>
        </div>
        <div class="contact-item">
          <i class="fas fa-envelope"></i> <!-- Email Icon -->
          <p>truenorthgeospatials@gmail.com</p>
        </div>
        <div class="contact-item">
          <i class="fas fa-globe"></i> <!-- Website Icon -->
          <p>[Insert Website URL]</p>
        </div>
      </div>
      <!-- Embedded Google Map -->
      <iframe
        class="map"
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3988.818575678745!2d36.84525!3d-1.17430!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMcKwMTAnMjcuNCJTIDM2wrA1MCc0Mi45IkU!5e0!3m2!1sen!2ske!4v1699999999999!5m2!1sen!2ske"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
      ></iframe>
    </section>
  </div>

  <footer>
    <p>&copy; 2025 True North Geospatials Ltd. All rights reserved.</p>
  </footer>

  <script>
    // Function to handle intersection observer for feedback boxes
    const animateFeedbackOnScroll = (entries, observer) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
        } else {
          entry.target.classList.remove('visible'); // Reset animation when out of view
        }
      });
    };

    // Set up Intersection Observer for feedback boxes
    const feedbackObserver = new IntersectionObserver(animateFeedbackOnScroll, {
      threshold: 0.5, // Trigger when 50% of the element is visible
    });

    // Observe feedback boxes
    const feedbackBoxes = document.querySelectorAll('.feedback-box');
    feedbackBoxes.forEach((box) => {
      feedbackObserver.observe(box);
    });

    // JavaScript to trigger the slide-in animation for service boxes (on page load)
    const serviceBoxes = document.querySelectorAll('.service-box');
    serviceBoxes.forEach((box, index) => {
      setTimeout(() => {
        box.style.opacity = '1';
        box.style.transform = 'translateX(0)';
      }, (index + 1) * 1000); // Each box slides in after 1 second
    });
  </script>
</body>
</html>
