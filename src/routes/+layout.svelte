<script>
  import "../app.css";
  import Footer from "./Footer.svelte";
  import NavBar from "./NavBar.svelte";
</script>
<div class=" mx-20">
  <NavBar/>
  <slot />
  <Footer/>
</div>