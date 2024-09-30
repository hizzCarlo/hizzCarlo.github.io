<script lang="ts">
  import type { PageData } from './$types';
  
  export let data: PageData;
</script>

<div class="container">
  <div class="content grid-container">
    <div class="image grid-item">
      <img src="/pf.png" alt="Profile Image">
      <ul class="image-details">
        <li><span>Name:</span> John Carlo A. Hizola</li>
        <li><span>Date of birth:</span> October, 31 2004</li>
        <li><span>Zip code:</span> 2110</li>
        <li><span>Nationality:</span> Filipino</li>
      </ul>
    </div>
    <div class="details grid-item">
      <h1>About <span>Me</span></h1>
      <p>Hi! I’m John Carlo, a 3rd-year Computer Science student at Gordon College. As someone passionate about technology, I’ve been fortunate enough to explore various aspects of software and web development while continuing to learn, especially in the field of Natural Language Processing (NLP). My journey as a student developer has been both challenging and rewarding, giving me the opportunity to turn my ideas into meaningful projects.</p>
      <br>
      <p>I’ve always been fascinated by how technology can solve real-world problems, and this curiosity led me to delve deeper into programming. Balancing my academic responsibilities with my personal interests in coding, I’ve grown from working on small-scale school projects to more ambitious initiatives, such as building a chatbot for user support.</p>
      <br>
      <p>Beyond my studies, I’m also passionate about digital art. I enjoy working on vector illustrations, animations, video editing, and creating artwork. These creative outlets allow me to express my artistic side and blend it with my technical skills.</p>
      <br>
      <p>When I’m not coding or creating digital art, I like to keep up with the latest trends in tech, spend time with family and friends, and dive into gaming or writing. I’m constantly learning and striving to sharpen my skills as I navigate the fast-evolving landscape of technology.</p>
      <br>
      <p>This portfolio is a reflection of my academic journey, passion for development, and the projects I’ve worked on so far. I’m excited to continue growing as a developer and contributing to innovative solutions that make a difference.</p>
    </div>
  </div>
</div>

<style>
  .container {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #00000000;
    color: #fff;
    padding-top: 60px; /* Add padding to avoid overlap with navbar */
    box-sizing: border-box;
  }
  .content {
    display: grid;
    grid-template-columns: 1fr 2fr;
    background-color: #1a1a1a;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
  }
  .image {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-right: 2rem;
  }
  .image img {
    border-radius: 50%;
    width: 150px;
    height: 150px;
    object-fit: cover;
  }
  .image-details {
    list-style: none;
    padding: 0;
    margin-top: 1rem;
    text-align: left;
  }
  .image-details li {
    margin-bottom: 0.5rem;
  }
  .image-details li span {
    font-weight: bolder;
    color: #ffcc00;
  }
  .details {
    max-width: 700px;
  }
  .details h1 {
    margin-bottom: 1rem;
  }
  .details ul {
    list-style: none;
    padding: 0;
  }
  .details ul li {
    margin-bottom: 0.5rem;
  }
  .download-cv {
    background-color: #ffcc00;
    color: #000;
    border: none;
    padding: 0.5rem 1rem;
    border-radius: 4px;
    cursor: pointer;
  }
  h1 span {
    color: #bd971bf9;
    font-weight: bolder;
  }
  h1 {
    font-weight: bolder;
    font-size: xx-large;
  }
</style>