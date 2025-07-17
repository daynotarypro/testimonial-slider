
<div id="testimonial-slider" style="max-width: 800px; margin: 0 auto; padding: 2em 1em; text-align: center; font-family: sans-serif;">
  <div class="testimonial active">
    <p>“Tunde was responsive, professional, and easy to work with. He met me within the hour and made the process stress-free.”</p>
    <strong>— Monica R., Long Beach</strong>
  </div>
  <div class="testimonial">
    <p>“I called around and nobody was available for a jail signing. Then I found Tunde at Day Notary Pro. He showed up early, handled everything cleanly, and even gave me a few pointers for next time. Real one.”</p>
    <strong>— Albert E., Fontana</strong>
  </div>
  <div class="testimonial">
    <p>“Tunde showed up to the hospital with everything ready. Kind, respectful, and extremely knowledgeable.”</p>
    <strong>— Kevin S., Bellflower</strong>
  </div>
</div>

<style>
  #testimonial-slider .testimonial {
    display: none;
    opacity: 0;
    transition: opacity 1s ease-in-out;
  }

  #testimonial-slider .testimonial.active {
    display: block;
    opacity: 1;
  }

  #testimonial-slider p {
    font-size: 1.25em;
    margin-bottom: 0.5em;
    line-height: 1.6;
  }

  #testimonial-slider strong {
    display: block;
    margin-top: 0.25em;
    font-size: 1em;
    color: #444;
  }
</style>

<script>
  let testimonials = document.querySelectorAll("#testimonial-slider .testimonial");
  let index = 0;

  function showNextTestimonial() {
    testimonials[index].classList.remove("active");
    index = (index + 1) % testimonials.length;
    testimonials[index].classList.add("active");
  }

  setInterval(showNextTestimonial, 6000); // rotates every 6 seconds
</script>
