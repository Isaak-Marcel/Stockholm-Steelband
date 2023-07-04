<script>
  import Burger from '../icons/align-justify.svelte'
  import CFA from './CFA.svelte'
  let showNav = false;

  const toggleNav = () => {
    showNav = !showNav;
  }
  
</script>

<nav class="mx-auto md:px-8 px-0 max-w-7xl">
  <div class="w-full flex justify-between items-center">
    <div class="">
       
      <a href="/" class="" >
        <img src='/images/Logo.png' alt="home"/>
      </a>
    </div>
    <ul class="hidden row-nav md:flex justify-evenly lg:w-96 md:w-80">
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
    <div class="hidden md:flex"><CFA /></div>
      <button class=" mr-4 svelte-ignore a11y-click-events-have-key-events lg:hidden md:hidden" on:click={toggleNav} >
        <Burger width={24} height={24} />
      </button>
  </div>
  
</nav>

<nav class="col-nav">
  {#if showNav}
  <div class="md:hidden flex flex-col colNav w-full z-20 absolute bg-black ">
    <a href="d" class="mx:pl-8 ">About us</a>
    <a href="d" class="mx:pl-8">About us</a>
    <a href="d" class="mx:pl-8">About us</a>
  </div>
{/if}
</nav>

<style>
  .row-nav a {
    display: flex;
    align-items: center;
    /* @apply mx-12 ; */
  }
  .colNav{

  }
  .colNav a{
      padding-left: 12px;
      padding: 10px ;
  }
</style>
