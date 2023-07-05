<script>
  import "../app.css";
  import Footer from "./Footer.svelte";
  import NavBar from "./NavBar.svelte";
</script>

  <NavBar/>
 <div >
  <slot />

  </div>
<div class=" mx-auto  max-w-7xl md:px-16 px-8 ">
  <!-- <Footer/> -->
</div>