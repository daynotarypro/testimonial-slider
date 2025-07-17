<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Day Notary Pro Testimonials</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #e5e5e5;
    }

    .testimonial-container {
      background-color: #e5e5e5;
      padding: 40px 20px;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 250px;
      position: relative;
    }

    .testimonial {
      max-width: 700px;
      text-align: center;
      font-size: 18px;
      color: #333;
      opacity: 0;
      transform: translateX(50px);
      transition: opacity 1s ease, transform 1s ease;
      position: absolute;
    }

    .testimonial.active {
      opacity: 1;
      transform: translateX(0);
      position: relative;
    }

    .author {
      margin-top: 15px;
      font-weight: bold;
      font-style: italic;
      color: #222;
    }
  </style>
</head>
<body>
  <div class="testimonial-container">
    <div class="testimonial active">
      “Tunde was responsive, professional, and easy to work with. He met me within the hour and made the process stress-free.”
      <div class="author">— Monica R., Long Beach</div>
    </div>
    <div class="testimonial">
      “I called around and nobody was available for a jail signing. Then I found Tunde at Day Notary Pro. He showed up early, handled everything cleanly, and even gave me a few pointers for next time. Real one.”
      <div class="author">— Albert E., Fontana</div>
    </div>
    <div class="testimonial">
      “Tunde showed up to the hospital with everything ready. Kind, respectful, and extremely knowledgeable.”
      <div class="author">— Kevin S., Bellflower</div>
    </div>
  </div>

  <script>
    const testimonials = document.querySelectorAll('.testimonial');
    let index = 0;

    setInterval(() => {
      testimonials[index].classList.remove('active');
      index = (index + 1) % testimonials.length;
      testimonials[index].classList.add('active');
    }, 5000);
  </script>
</body>
</html>
