<script lang="ts">
  import type { PageData } from './$types';
  
  export let data: PageData;
</script>

<div class="container">
  <div class="content">
    <div class="image">
      <img src="/pf.png" alt="Profile Image">
      <ul class="image-details">
        <li><strong>Name:</strong> John Carlo A. Hizola</li>
        <li><strong>Date of birth:</strong> October, 31 2004</li>
        <li><strong>Zip code:</strong> 2110</li>
        <li><strong>Nationality:</strong> Filipino</li>
      </ul>
    </div>
    <div class="details">
      <h1>About Me</h1>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>

      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
    </div>
  </div>
</div>

<style>
  .container {
    font-family: Arial, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 80vh;
    background-color: #00000000;
    color: #fff;
  }
  .content {
    display: flex;
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
</style>