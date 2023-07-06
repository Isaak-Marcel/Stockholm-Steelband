<script>
  import Burger from '../icons/align-justify.svelte'
  import CFA from './CFA.svelte'
  let showNav = false;

  const toggleNav = () => {
    showNav = !showNav;
  }
  
</script>


<nav class=" bg-white">
  <div class="mx-auto md:px-8 px-0 max-w-7xl bg-white">
    <div class="w-full flex justify-between items-center">
      <div class="flex justify-center items-center">
        <a href="/" class="" >
          <img src='/images/Logo.png' alt="home"/>
        </a>
      </div>
      <ul class="hidden text-black font-semibold row-nav md:flex justify-evenly lg:w-96 md:w-80">
        <a href="#Om-Oss">
          <li>Om oss</li>
        </a>
        <a href="#Om-Steelband">
          <li>Om Steelband</li>
        </a>
        <a href="#Boka-oss">
          <li>Kontakta Oss</li>
        </a>
      </ul>
      <a href="" class="hidden lg:block"><span style="padding: 0" class="pb-4 font-semibold text-black">info@stockholmsteelband.se</span></a>
      <div class="hidden md:flex"><CFA color='black' /></div>
        <button class=" mr-4 svelte-ignore a11y-click-events-have-key-events lg:hidden md:hidden" on:click={toggleNav} >
          <Burger color='black' width={24} height={24} />
        </button>
    </div>
  </div>
  
</nav>
<a class="md:hidden bottom-0 w-full text-xl font-bold text-center z-20 fixed bg-yellow-600 p-3" href='#Boka-oss'>
  Boka Oss
  </a>
<nav class="col-nav">
   <!--I want this a tag to stick to the buttom of the screen at all time on md devices  -->
  
  {#if showNav}
  <div class="md:hidden flex flex-col colNav w-full z-20 absolute bg-black ">
    <a href="#Om-Oss" class="mx:pl-8 ">Om oss</a>
    <a href="#Om-Steelband" class="mx:pl-8">Om Steelband</a>
    <a href="#Boka-oss" class="mx:pl-8">Kontakta Oss</a>
  </div>
{/if}
</nav>

<style>
  .row-nav a {
    display: flex;
    align-items: center;
    /* @apply mx-12 ; */
  }
 
  .colNav a{
      padding-left: 12px;
      padding: 13px ;
  }
</style>
