<script>
    export let activePage = '';
  </script>
  
  <nav>
    <ul>
      <li class={activePage === 'home' ? 'active' : ''}><a href="/">Home</a></li>
      <li class={activePage === 'about' ? 'active' : ''}><a href="/about">About</a></li>
      <li class={activePage === 'contact' ? 'active' : ''}><a href="/contact">Contact</a></li>
      <li class={activePage === 'portfolio' ? 'active' : ''}><a href="/portfolio">Portfolio</a></li>
    </ul>
  </nav>
  
  <style>
    nav {
      background-color: #333;
      padding: 1rem;
    }
    ul {
      list-style: none;
      display: flex;
      gap: 1rem;
    }
    li {
      color: white;
    }
    li.active a {
      font-weight: bold;
    }
    a {
      color: white;
      text-decoration: none;
    }
  </style>