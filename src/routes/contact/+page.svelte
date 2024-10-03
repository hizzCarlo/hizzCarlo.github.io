<script lang="ts">
  import type { PageData } from './$types';
  export let data: PageData;
  import '@fortawesome/fontawesome-free/css/all.min.css';
  import 'flowbite/dist/flowbite.css';
</script>
<!-- contact page -->
<div class="container">
  <div class="relative z-10">
    <div class="image-container">
      <div class="image-background">
        <img src="/pic2.png" alt="John Carlo">
      </div>
    </div>
      
    <div class="contact-container">
      <h1>Contact <span>Me.</span></h1>
      <p>Get in touch to get the ball rolling</p>
      <div class="contact-info"><!-- clickable contacts -->
        <div class="contact-item">
          <a href="https://mail.google.com/mail/u/0/?hl=en-GB#inbox" class="btn btn-primary">
            <i class="fas fa-envelope"></i>
            <p>EMAIL</p>
            <span>202211255@gordoncollege.edu.ph</span>
          </a>
        </div>
        <div class="contact-item">
          <a href="tel: +639673606059" class="btn btn-primary">
            <i class="fas fa-phone"></i>
            <p>PHONE</p>
            <span>+63 (0) 9673 606059</span>
          </a>
        </div>
        <div class="contact-item">
          <a href="https://www.facebook.com/johncarlo.hizola.9/" class="btn btn-primary">
            <i class="fa-brands fa-facebook"></i>
            <p>FACEBOOK</p>
            <span>Johncarlo Hizola</span>
          </a>
        </div>
        <div class="contact-item">
          <a href="https://x.com/JohnHizola70295" class="btn btn-primary">
            <i class="fa-brands fa-twitter"></i>
            <p>TWITTER</p>
            <span>John Carlo Hizola</span>
          </a>
        </div>
        <div class="contact-item">
          <a href="https://github.com/hizzCarlo" class="btn btn-primary">
            <i class="fa-brands fa-github"></i>
            <p>GITHUB</p>
            <span>Hizola, John Carlo</span>
          </a>
        </div>
        <div class="contact-item">
          <a href="https://www.instagram.com/jc.hiz/" class="btn btn-primary">
            <i class="fa-brands fa-square-instagram"></i>
            <p>INSTAGRAM</p>
            <span>jc.hiz</span>
          </a>
        </div>
      </div>
    </div>
  </div>
</div>

<style>
  .container {
    font-family: Arial, sans-serif;
    max-width: 800px;
    margin: 0 auto;
    background-color: white;
    padding: 1rem;
    top: 4.5rem;
    border-radius: 8px;
    z-index: 4;
    position: relative;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  .content {
    position: relative;
    z-index: 2;
  }
  .contact-container {
    text-align: center;
    padding: 1rem;
  }
  .contact-info {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1rem;
    margin-top: 2rem;
  }
  /* for larger screen */
  @media (max-width: 800px) {
    .contact-info {
      grid-template-columns: repeat(2, 1fr);
    }
  }
  /* for smaller screen */
  @media (max-width: 500px) {
    .contact-info {
      grid-template-columns: 1fr;
    }
  }

  .contact-item {
    text-align: center;
    padding: .5rem;
  }
  .contact-item i {
    font-size: 2rem;
    color: #000000f9;
    transition: transform 0.3s ease, color 0.3s ease; /* transition for smoother effect */
  }
  .contact-item i:hover {
    transform: scale(1.2); /* make the icon bigger */
    color: #bd971bf9; 
  }
  .contact-item p {
    margin: 0.5rem 0;
    color: #bd971bf9;
  }
  .contact-item a {
    color: #000;
    text-decoration: none;
  }
  .image-container {
    display: flex;
    justify-content: center; 
    margin-bottom: 1rem; 
  }
  .image-background {
    position: relative;
    width: 250px;
    height: 250px;
    background-color: #bd971bf9;
    border-top-left-radius: 80%;
    border-top-right-radius: 200%;
    border-bottom-left-radius: 90%;
    border-bottom-right-radius: 100%;
    z-index: 3;
    display: flex;
    overflow: hidden; 
    justify-content: center;
    align-items: center;
  }
  .image-background img {
    border-radius: 60px;
    max-width: 80%;
  }
  h1 span {
    color: #bd971bf9;
    font-weight: bolder;
  }
  h1 {
    font-weight: bolder;
    font-size: larger;
  }
</style>