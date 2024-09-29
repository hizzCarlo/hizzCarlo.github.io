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


<div class="bottom-box">
    
</div>

<style>
    nav {
        background-color: transparent;
        padding: 1rem;
        display: flex;
        font-family: Arial, sans-serif;
        justify-content: center; 
        z-index: 3; 
        position: relative; 
    }
    ul {
        list-style: none;
        display: flex;
        gap: 1rem;
    }
    li {
        color: rgb(255, 255, 255);
    }
    li.active a {
        color: #bd971b;
        font-weight: bold;
        text-decoration: underline; 
    }
    a {
        color: rgb(255, 255, 255);
        text-decoration: none;
    }
    .bottom-box {
        position: fixed;
        bottom: 0;
        left: 0; 
        height: 20vh;
        width: 100%;
        background-color: #fefefe;
        text-align: center;
        padding: 1rem;
        box-shadow: 0 -2px 5px rgba(0, 0, 0, 0.1);
        z-index: -1; 
    }
</style>