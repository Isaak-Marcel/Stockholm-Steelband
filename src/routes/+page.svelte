<script>
  import Contact from "./Contact.svelte";
  import OmOss from "./OmOss.svelte";
  import OmSteelband from "./OmSteelband.svelte";
  import SoicalMedia from "./SoicalMedia.svelte";
  import Video from "./Video.svelte";
  import OmStockholmSteelband from "./OmStockholmSteelband.svelte";
  import YoutubeVideoEmbed from "./YoutubeVideoEmbed.svelte";

</script>

<meta
  name="description"
  content="Stockholm Steelband är ett oljefat band i stockholm som spelar på event, bröllop, företagsfester, festivaler och andra tillställningar. "
/>


<svelte:head>
  <title>Stockholm Steelband</title>
  <link rel="canonical" href="https://www.stockholmsteelband.se" />
</svelte:head>

<Video />
<div class="mx-auto overflow-x-hidden max-w-7xl md:px-16 px-8">
  <SoicalMedia />
  <OmOss />
  <OmSteelband />
  <YoutubeVideoEmbed />
  <OmStockholmSteelband />
  <Contact />
</div>
