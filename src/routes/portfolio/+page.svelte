<script lang="ts">
    import type { PageData } from './$types';
    
    export let data: PageData;

    // Example data for school works
    const schoolWorks = [
        { title: 'Project 1', description: 'Description of project 1', year: 2021 },
        { title: 'Assignment 1', description: 'Description of assignment 1', year: 2022 },
        { title: 'Project 2', description: 'Description of project 2', year: 2023 },
        // Add more works as needed
    ];
</script>

<div class="container">
  <div class="relative z-10">
    <h1>Portfolio Page</h1>
    <p>Welcome to the portfolio page.</p>
    
    <section>
      <h2>Gallery of School Works</h2>
      <p>Display a gallery of your schoolwork from the past 3 years up to the present. This can include projects, assignments, and other relevant work.</p>
      <div class="gallery">
        {#each schoolWorks as work}
          <div class="work-item">
            <h3>{work.title} ({work.year})</h3>
            <p>{work.description}</p>
          </div>
        {/each}
      </div>
    </section>
  </div>
</div>

<style>
  .container {
    max-width: 800px;
    margin: 0 auto;
    background-color: white;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  .gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1rem;
  }
  .work-item {
    border: 1px solid #ccc;
    padding: 1rem;
    border-radius: 8px;
    background-color: #f9f9f9;
  }
</style>