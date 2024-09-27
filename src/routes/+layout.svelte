<script>
    import Navbar from '$lib/Navbar.svelte';
    import { page } from '$app/stores';
  
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
  
  <slot />