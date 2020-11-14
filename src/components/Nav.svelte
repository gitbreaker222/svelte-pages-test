<script>
  let isOpen = false;
  const toggleNav = () => isOpen = !isOpen
  const deferClose = (event) => {
    const {target} = event
    
    if (target.tagName === 'A') {
      window.setTimeout(() => {
        isOpen = false;
      }, 200)
    }
  }
</script>

<nav class:isOpen={isOpen}>
  <div class="pages" on:click={deferClose}>
    <a href="/">Home</a>
    <a href="/about" >About</a>
  </div>
  <button on:click={toggleNav}>
    {#if isOpen}
    X
    {:else}
    📑
    {/if}
  </button>
</nav>

<style>
  nav {
    position: fixed;
    right: 0;
    bottom: 0;
    left: 0;
    height: var(--nav-size);
    display: grid;
  }
  
  nav.isOpen {
    height: 100vh;
    background: #e4e4e4;
  }

  .pages {
    display: none;
  }
  .isOpen .pages {
    display: grid;
    align-content: flex-start;
  }

  button {
    justify-self: center;
    position: fixed;
    bottom: .2rem;
  }

  a {
    display: inline-block;
    min-width: 6rem;
    margin: .5rem;
    padding: 1rem;
    border: 1px solid currentColor;
  }
</style>