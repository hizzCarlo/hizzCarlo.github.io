<script lang="ts">
</script>
<!-- home page -->
<div class="container">
  <div class="about-page">
    <div class="content-box">
      <main class="main-content">
        <div class="intro">
          <h2>Hello, Welcome</h2>
          <h1>I am Hizola, John Carlo</h1>
          <p>
            A student at Gordon College in the Computer Studies Department. and I’m currently taking a course on Bachelor of Science in Computer Science</p>
        </div>
        <div class="image-container">
          <div class="image-background">
            <img src="/pic2.png" alt="John Carlo">
          </div>
        </div>
      </main>
    </div>
  </div>
</div>

<style>
  /* import custom style */
  @import '../styles/custom.css'; 
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: Arial, sans-serif;
    height: 90vh; 
  }
  .about-page {
    background-color: transparent;
    color: #333;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 80vh;
  }
  .content-box {
    background-color: rgb(255, 255, 255);
    padding: 2rem;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    max-width: 990px;
    width: 100%;
  }
  .main-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .intro {
    max-width: 50%;
  }
  .intro h2 {
    color: #bd971b;
    font-size: xx-large;
  }
  .intro h1 {
    font-size: 2.5rem;
    margin: 1rem 0;
  }
  .intro p {
    margin: 1rem 0;
  }
  
  .image-container {
    position: relative;
    width: 380px;
    height: 390px;
    background-color: #bda21baa;
    border-top-left-radius: 50%;
    border-top-right-radius: 20%;
    border-bottom-left-radius: 20%;
    border-bottom-right-radius: 50%;
  }
  .image-background {
    position: relative;
    width: 400px;
    height: 400px;
    background-color: #bd971b3a;
    border-top-left-radius: 50%;
    border-top-right-radius: 20%;
    border-bottom-left-radius: 20%;
    border-bottom-right-radius: 50%;
    z-index: 3;
    position: relative;
    display: flex;
    overflow: hidden; 
    justify-content: center;
    align-items: center;
  }
  .image-background img {
    border-radius: 60px;
    max-width: 80%;
  }
  
  @media (max-width: 800px) {
    .main-content {
      flex-direction: column;
    }
    .intro {
      max-width: 100%;
      text-align: center;
    }
    .image-container {
      width: 300px;
      height: 310px;
    }
    .image-background {
      width: 320px;
      height: 320px;
    }
  }
  
  @media (max-width: 500px) {
    .image-container {
      width: 250px;
      height: 260px;
    }
    .image-background {
      width: 270px;
      height: 270px;
    }
  }
</style>