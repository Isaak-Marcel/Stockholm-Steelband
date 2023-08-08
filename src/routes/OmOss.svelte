<script>
  import { fade } from "svelte/transition";
  import RigthArrowIcon from "../icons/Rigth-arrow-icon.svelte";
  import LeftArrowIcon from "../icons/Left-arrow-Icon.svelte";
  import { onMount } from "svelte";

  const carouselPhotos = [
    "sliderImages/I rödpaljett gruppbild.jpg",
    "sliderImages/Isabelle.jpg",
    "sliderImages/pannor utan logga.jpg",
    "sliderImages/Gruppbild kimono 2.jpg",
    "sliderImages/gruppbild regnbåge.jpg",
    "sliderImages/Johanna.jpg",
    "sliderImages/Jungfru.jpg",
    "sliderImages/trädgårnden stor.jpg",
  ];

  let index = 0;

  const switchImages = () => {
    setInterval(next, 3000);
  };

  onMount(switchImages);

  const next = () => {
    index = (index + 1) % carouselPhotos.length;
  };

  const previous = () => {
    index = (index - 1 + carouselPhotos.length) % carouselPhotos.length;
  };
</script>

<section class="pt-14 pb-8" id="Om-Oss">
  <div class="lg:flex lg:justify-center lg:items-center gap-8">
    <div class="basis-2/4 lg:pl-10 lg:justify-end lg:block flex justify-center">
      <h2 class="lg:block hidden opacity-0 pb-2">Om Musiken</h2>
      <div class="relative lg:w-auto w-[470px] lg:h-[278px] h-[238px]">
        {#each [carouselPhotos[index]] as src (index)}
          <img
            transition:fade
            {src}
            class="h-full w-full absolute object-scale-down"
            alt=""
          />
        {/each}
        <button class="next-button" on:click={next}
          ><RigthArrowIcon width={40} height={40} /></button
        >
        <button class="previous-button" on:click={previous}
          ><LeftArrowIcon width={40} height={40} /></button
        >

        <div class="absolute mb-2 flex justify-center w-full mx-auto bottom-0">
          {#each carouselPhotos as photo, i}
            <button
              class=" self-center dot {i === index ? 'active-dot' : ''}"
              on:click={() => (index = i)}
            />
          {/each}
        </div>
      </div>
    </div>

    <div
      class="basis-2/4 lg:pl-10 lg:pt-4 pt-10 lg:block flex-col items-center flex"
    >
      <h2
        style="text-transform: none;"
        class="pb-2 h2Small lg:text-left text-center"
      >
        Om musiken
      </h2>
      <p class="p2 lg:text-left lg:p-0 text-center lg:mb-6 mb-5">
        Musiken består av karibiska rytmer så som calypso och soca, med en
        blandad repertoar av traditionella låtskatter från Trinidad and Tobago
        och arrangemang av kända hits. Vi spelar på festivaler och företagsevent,
        firmafester – små som stora, privata fester, bröllop, dop,
        födelsedagsfirande, lokala gatufester, folkparker och karnevaler till
        större event i Stadshuset, Pride och Polarprisutdelning. I samarbete med
        uppdragsgivaren skräddarsyr vi våra spelningar för att anpassa oss till
        era önskemål och upplägg.
      </p>
      <!-- <a href="#Boka-oss" class="px-6 text-center bg-cYellow py-2 rounded"
        >Boka oss</a
      > -->
    </div>
  </div>
</section>

<style>
  .next-button,
  .previous-button {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    z-index: 1;
    background-color: transparent;
    cursor: pointer;
  }

  .previous-button {
    left: -44px;
  }

  .next-button {
    right: -44px;
  }

  @media (max-width: 600px) {
    .previous-button {
      left: 14px;
    }
    .next-button {
      right: 14px;
    }
  }

  .dot {
    width: 8px;
    height: 8px;
    background-color: black;
    border-radius: 50%;
    margin: 0 4px;
    cursor: pointer;
  }

  .active-dot {
    background-color: white;
  }
</style>
