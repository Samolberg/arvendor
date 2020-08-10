<script>
    export let items = [];
</script>

<header class="navbar-header">
    <div class="navbar-header-content">
        <div class="navbar-logo">
            Arvendor logo goes here
        </div>
        <nav class="navbar-items">
            <ul>
                {#each items as item}
                    <li>
                        <a href={item.link}>{item.name}</a>
                    </li>
                {/each}
            </ul>
        </nav>
    </div>
</header>

<style>
  header * {
    font-size: 18px;
  }
  
  .navbar-header {
    position: fixed;
    width: 100%;
    z-index: 1000;
    top: 0;
    display: block;
    
    background: #eee;
    opacity: 0.9;
  }
  
  .navbar-header-content {
    width: 80%;
    max-width: 1000px;
    margin: 20px auto 20px;
    padding: 0 32px 0;
    display: flex;
    overflow: hidden;
    align-items: center;
    justify-content: space-between;
  }
  
  nav {
    display: block;
  }
  
  nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
  }
  
  nav ul li {
    display: inline;
  }
  
  nav ul li a {
    padding: 10px 20px;
    margin: 10px 0;
  }
</style>
