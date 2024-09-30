<script>
    import Navbar from '$lib/Navbar.svelte';
    import { page } from '$app/stores';
    import '../styles/custom.css'; // Import the custom CSS

    let activePage = '';

    $: {
        const path = $page.url.pathname;
        if (path === '/') {
            activePage = 'home';
        } else if (path.startsWith('/about')) {
            activePage = 'about';
        } else if (path.startsWith('/contact')) {
            activePage = 'contact';
        } else if (path.startsWith('/portfolio')) {
            activePage = 'portfolio';
        }
    }
</script>

<Navbar {activePage} />

<div class="stars">
    {#each Array(50) as _, i}
        <div class="star" style="--top-offset: {Math.random() * 100}vh; --fall-duration: {6 + Math.random() * 6}s; --fall-delay: {Math.random() * 10}s; --star-tail-length: {5 + Math.random() * 2.5}em;"></div>
    {/each}
</div>

<div class="content grid-container">
    <slot />
</div>

<style>
  .content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    min-height: 80vh; /* Ensure it takes full viewport height */
  }

  @media (max-width: 768px) {
    .content {
      padding: 1rem;
    }
  }
</style>