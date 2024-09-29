<script lang="ts">
    import type { PageData } from './$types';
    import { onMount } from 'svelte';
    
    export let data: PageData;
    
    // Example data for school works
    const schoolWorks = [
        { title: 'Navigation-Bar', description: 'A basic navigation bar using HTML and CSS', year: 2024 },
        { title: 'Basic-Calculator', description: 'A basic Calculator using HTML, CSS, and JS', year: 2024 },
        { title: 'Project-management-System', description: 'Simple CRUD system using HTML, CSS, and JS', year: 2024 },
        { title: 'Image-Gallery', description: 'Image-Gallery for storing and editing images using HTML, Typescript, SCSS, and PHP', year: 2024 },
        { title: '3D-Shape-Rendering', description: '3D rendering a cube and a pyramid using Python', year: 2022 },
        { title: 'Advance-Calculator', description: 'Advance Calculator using python', year: 2022 },
        { title: '3D-vector-line-projection', description: 'three-dimensional Cartesian coordinate system, generated using Python', year: 2022 },
        { title: 'basic-turtle-graphic', description: 'A simple turtle graphic using python', year: 2022 },
        { title: '3D-Letter--Rendering', description: '3d rendering Letter (H, P, R, T) using python', year: 2022 },
        { title: 'Fitness-web', description: 'fitness website using php', year: 2022 },
        // Add more works as needed
    ];
    
    let showPopup = false;
    let selectedImage = '';
    
    function openPopup(imageSrc: string) {
        selectedImage = imageSrc;
        showPopup = true;
    }
    
    function closePopup() {
        showPopup = false;
        selectedImage = '';
    }
</script>
<div class="container">
  <h2>Other Projects</h2>
  <div class="container1">
    <div class="gallery1">

      <div class="gallery-item" on:click={() => openPopup('/web1.png')}>
        <img src="/web1.png" alt="Image 1">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/web2.png')}>
        <img src="/web2.png" alt="Image 2">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/about.jpg')}>
        <img src="/about.jpg" alt="Image 3">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/contact.jpg')}>
        <img src="/contact.jpg" alt="Image 4">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/home.jpg')}>
        <img src="/home.jpg" alt="Image 5">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/store.jpg')}>
        <img src="/store.jpg" alt="Image 6">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/logo.jpg')}>
        <img src="/logo.jpg" alt="Image 7">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/drawing baby boy.jpeg')}>
        <img src="/drawing baby boy.jpeg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/drawing baby girl.jpeg')}>
        <img src="/drawing baby girl.jpeg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/drawing girl.jpeg')}>
        <img src="/drawing girl.jpeg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/drawing boy.jpeg')}>
        <img src="/drawing boy.jpeg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/drawing teen girl.jpeg')}>
        <img src="/drawing teen girl.jpeg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/drawing teen boy.jpeg')}>
        <img src="/drawing teen boy.jpeg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/drawing women.jpeg')}>
        <img src="/drawing women.jpeg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/drawing man.jpeg')}>
        <img src="/drawing man.jpeg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/drawing old lady.jpeg')}>
        <img src="/drawing old lady.jpeg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/drawing old man.jpeg')}>
        <img src="/drawing old man.jpeg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/baby boy vector (Finished).jpg')}>
        <img src="/baby boy vector (Finished).jpg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/baby girl vector (Finished).jpg')}>
        <img src="/baby girl vector (Finished).jpg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/Girl Vector (Finished).jpg')}>
        <img src="/Girl Vector (Finished).jpg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/boy vector (Finished).jpg')}>
        <img src="/boy vector (Finished).jpg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/teen girl Vector (Finished).jpg')}>
        <img src="/teen girl Vector (Finished).jpg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/teen boy vector (Finished).jpg')}>
        <img src="/teen boy vector (Finished).jpg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/women Vector (Finished).jpg')}>
        <img src="/women Vector (Finished).jpg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/man vector (Finished).jpg')}>
        <img src="/man vector (Finished).jpg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/old lady Vector (Finished).jpg')}>
        <img src="/old lady Vector (Finished).jpg" alt="Image 8">
      </div>
      <div class="gallery-item" on:click={() => openPopup('/old man vector (Finished).jpg')}>
        <img src="/old man vector (Finished).jpg" alt="Image 8">
      </div>
    </div>
  </div>
  <div class="container2">
    <div class="relative z-10">
      
      <section>
        <h2>GitHub Projects</h2>
        <div class="gallery">
          {#each schoolWorks as work}
            <div class="work-item" on:click={() => window.location.href = `https://github.com/hizzCarlo/${work.title}`}>
              <h3>{work.title} ({work.year})</h3>
              <p>{work.description}</p>
              <a href={`https://github.com/hizzCarlo/${work.title}`}>Learn more</a>
            </div>
          {/each}
        </div>
      </section>
    </div>
  </div>
</div>
{#if showPopup}
  <div class="popup">
    <div class="popup-content">
      <button class="close-button" on:click={closePopup}>X</button>
      <img src={selectedImage} alt="Full Image">
    </div>
  </div>
{/if}
<style>
  .container {
    max-width: 70%;
    margin: 0 auto;
    background-color: rgba(0, 0, 0, 0.348);
    padding: 2rem;
    top: 4.5rem;
    border-radius: 8px;
    z-index: 2;
    position: relative;
    box-shadow: 0 0 10px rgba(255, 255, 255, 0.1);
    font-family: Arial, sans-serif;
    margin-bottom: 1rem; /* Add margin to separate the containers */
  }
  .container1 {
    overflow-x: auto;
    overflow-y: hidden;
    white-space: nowrap;
    padding-bottom: .5rem;
  }
  .gallery {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1rem;
  }
  /* Scrollbar styles */
  .container1::-webkit-scrollbar {
    height: 8px; /* Adjust the height of the scrollbar */
  }

  .container1::-webkit-scrollbar-track {
    background: transparent; /* Transparent background for the track */
  }

  .container1::-webkit-scrollbar-thumb {
    background-color: rgba(255, 166, 0, 0.501); /* Orange color for the scrollbar thumb */
    border-radius: 10px; /* Rounded corners for the scrollbar thumb */
    border: 2px solid transparent; /* Add some space around the thumb */
    background-clip: content-box; /* Clip the background to the content box */
    transition: background-color 0.3s ease, height 0.3s ease; /* Smooth transition for the color and size */
  }

  .container1::-webkit-scrollbar-thumb:hover {
    background-color: darkorange; /* Change color when hovered */
    height: 12px; /* Make the scrollbar thumb bigger when hovered */
  }

  .gallery1 {
    display: inline-block;
    white-space: nowrap;
  } 
  .gallery-item {
    display: inline-block;
    width: 200px; /* Set a fixed width for the images */
    height: 200px; /* Set a fixed height for the images */
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.2s;
    margin-right: 1rem; /* Add some space between images */
    overflow: hidden; /* Hide overflow */
    cursor: pointer; /* Change cursor to pointer */
  }
  .gallery-item img {
    width: 100%;
    height: 100%;
    object-fit: cover; /* Ensure the image covers the container */
  }
  .gallery-item:hover {
    transform: scale(1.05);
  }
  .work-item {
    border: 1px solid #ccc;
    padding: 1rem;
    border-radius: 8px;
    background-color: #f9f9f9;
    cursor: pointer;
  }
  .work-item h3 {
    color: #000000;
    font-weight: bolder;
  }
  .work-item p {
    font-size: 0.7rem;
  }
  .work-item a {
    display: block;
    margin-top: 0.5rem;
    color: #ffcc00;
    text-decoration: none;
  }
  .work-item a:hover {
    text-decoration: underline;
  }
  h2 {
    color: #f9f9f9;
    font-weight: bolder;
    font-size: xx-large;
  }
  .container2{
    padding-top: 1rem;
  }
  .popup {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.8);
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1000;
  }
  .popup-content {
    position: relative;
    background-color: #fff;
    padding: 1rem;
    border-radius: 8px;
    max-width: 90%;
    max-height: 90%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .popup-content img {
    max-width: 100%;
    max-height: 80vh; /* Limit the height of the image */
    object-fit: contain; /* Ensure the image maintains its aspect ratio */
    border-radius: 8px;
  }
  .close-button {
    position: absolute;
    top: 10px;
    right: 10px;
    background-color: #ff0000;
    color: #fff;
    border: none;
    border-radius: 50%;
    width: 30px;
    height: 30px;
    cursor: pointer;
    font-size: 1rem;
    display: flex;
    justify-content: center;
    align-items: center;
  }
</style>