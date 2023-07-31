<script>
  import Burger from '../icons/align-justify.svelte'
  import CFA from './CFA.svelte'
  let showNav = false;
  import EmailIcon from '../icons/Email-forward-icon.svelte'

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
      <ul class="hidden gap-8  text-black font-semibold row-nav  lg:flex justify-evenly lg:w-[600px] md:w-80 ">
        <a href="#Om-Oss">
          <li>Om Musiken</li>
        </a>
        <a href="#Om-Steelband">
          <li>Om Instrumenten</li>
        </a>
        <a href="#omStockholmSteelband">
          <li>Om oss</li>
        </a>
        <a href="#showreel">
          <li>Showreel</li>
        </a>
        <a href="#Boka-oss">
          <li>Kontakta oss</li>
        </a>
      </ul>
      <div class="hidden lg:flex"><CFA color='black' /></div>
        <div class="flex">
        <a class="pr-6" href="mailto:info@stockholmsteelband.se"> <EmailIcon color='black' width={24} height={24}/> </a>
          <button class=" mr-4 svelte-ignore a11y-click-events-have-key-events lg:hidden " on:click={toggleNav} >
            <Burger color='black' width={24} height={24} />
          </button>
        </div>
    </div>
  </div>
  
</nav>
<a class="md:hidden bottom-0 w-full text-xl font-bold text-center z-20 fixed bg-yellow-600 p-3" href='#Boka-oss'>
  Boka Oss
  </a>
<nav class="col-nav">
   <!--I want this a tag to stick to the buttom of the screen at all time on md devices  -->
  
  {#if showNav}
  <div class="lg:hidden flex flex-col colNav w-full z-20 absolute bg-black ">
    <a href="#Om-Oss" class="mx:pl-8 ">Om Musiken</a>
      <a href="#Om-Steelband" class="mx:pl-8">Om Instrumenten</a>
      <a href="#omStockholmSteelband">
        Om oss
      </a>
      <a href="#showreel">
        Showreel
      </a>
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


  @media (max-width: 640px) {
    .navEmail{
      
      visibility: hidden;
    }
  }
  
  @media (max-width: 575px) {
    .navEmail{
    }
  }
</style>
