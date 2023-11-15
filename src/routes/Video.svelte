<script>
  let isMuted = true;
  import Volume from "../icons/volume.svg.svelte";
  import VolumeX from "../icons/volume-x.svg.svelte";

  function toggleMute() {
    isMuted = !isMuted;
  }
</script>

<section class="sectionReal">
  <video
    bind:muted={isMuted}
    autoplay
    playsinline
    disablepictureinpicture
    loop
    class="w-full object-cover absolute -z-10 min"
  >
    <track kind="captions" />
    <source
      src="https://firebasestorage.googleapis.com/v0/b/stockholm-steelband.appspot.com/o/Kort%20till%20hemsidan%20h%C3%B6gst%20upp%20utan%20Meme%203%20filmer.mp4?alt=media&token=b9714ff0-657e-4654-b980-86dec25de7ba"
    />
  </video>

  <div class="cont absolute">
    <button class="absolute right-0 pt-8" on:click={toggleMute}>
      {#if isMuted}
        <VolumeX />
      {:else}
        <Volume />
      {/if}
    </button>
  </div>
</section>

<div
  class=" MainWrapper flex flex-col justify-center items-center relative z-2"
>
  <div class=" text-center z-10">
    <!-- <h2 class="h2 mx-auto pb-4">Stockholm Steelband</h2> -->

    <p class="steelP p">
      Stockholm Steelband är ett oljefatsband som har sin givna plats när det
      kommer till att sprida dansglädje och feststämning. Karibiska rytmer för
      både lugnare mingelmusik och smittande, oemotståndlig dansmusik. Vi
      skräddarsyr våra spelningar för både stora och små event.
    </p>
  </div>
  <p class="pt-4 text-center font-semibold">Välkommen med din förfrågan!</p>
</div>

<style>
  .sectionReal {
    position: relative;
    overflow: hidden;
    height: 490px;
  }

  .sectionReal::after {
    content: "";
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 40%;
    background: linear-gradient(transparent, black);
    z-index: 1;
  }

  video {
    height: 750px;
  }
  .sectionReal {
    height: 700px;
  }

  /* Adjust the screen width value as needed */
  @media (max-width: 768px) {
    video {
      height: 600px;
    }
    .sectionReal {
      height: 400px;
    }
  }

  @media (max-width: 576px) {
    video {
      height: 550px;
    }
    .sectionReal {
      height: 520px;
    }
  }
</style>
