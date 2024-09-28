<script lang="ts">
  import type { PageData } from './$types';
  
  export let data: PageData;
</script>

<div class="container">
  <div class="relative z-10">
    <h1>Contact Page</h1>
    <p>Welcome to the contact page.</p>
    <p>Contact Information:</p>
    <ul>
      <li><a href="https://github.com/yourusername" target="_blank">GitHub</a></li>
      <li><a href="https://linkedin.com/in/yourusername" target="_blank">LinkedIn</a></li>
      <li><a href="https://facebook.com/yourusername" target="_blank">Facebook</a></li>
    </ul>
    <p>Email: <a href="mailto:youremail@example.com">youremail@example.com</a></p>
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
</style>