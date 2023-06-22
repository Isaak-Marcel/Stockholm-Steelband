<script>
  import Burger from '../icons/align-justify.svelte'
  import CFA from './CFA.svelte'
  let showNav = false;

  const toggleNav = () => {
    showNav = !showNav;
  }
  
</script>

<nav class="mx-auto md:px-16 px-8 max-w-7xl">
  <div class="w-full flex justify-between items-center">
    <div>
       
      <a href="/" >
        <img src='/images/Logo.png' alt="home"/>
      </a>
    </div>
    <ul class="hidden row-nav md:flex justify-evenly ">
      <a href="d">
        <li>About us</li>
      </a>
      <a href="d">
        <li>About us</li>
      </a>
      <a href="d">
        <li>About us</li>
      </a>
    </ul>
    <CFA />
      <button class="svelte-ignore a11y-click-events-have-key-events lg:hidden md:hidden" on:click={toggleNav} >
        <Burger width={24} height={24} />
      </button>
  </div>
  
</nav>

<nav class="col-nav">
  {#if showNav}
  <div class="md:hidden flex flex-col absolute bg-black ">
    <a href="d" class="pl-8 ">About us</a>
    <a href="d" class="pl-8">About us</a>
    <a href="d" class="pl-8">About us</a>

  </div>
{/if}
</nav>

<style>
  .row-nav a {
    display: flex;
    align-items: center;
    margin: 0 30px 0 30px;
  }
</style>
