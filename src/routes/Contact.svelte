<script>
  import PhoneIcon from "../icons/phone-call-icon.svelte";
  import EmailIcon from "../icons/Email-forward-icon.svelte";
</script>

<section
  id="Boka-oss"
  class="pb-20 mb-24 mt-14 outline rounded-2xl mx-auto max-w-4xl pb"
>
  <h2 class="h2Small text-center pt-8 lg:py-14">Boka Oss</h2>
  <div
    class="md:flex-row flex-col justify-center items-center gap-8 flex px-24"
  >
    <div
      class="md:w-1/2 w-full flex items-center lg:justify-start justify-center lg:pt-0 lg:pb-4 pt-10"
    >
      <ul class="pt-4">
        <div class="flex gap-2">
          <EmailIcon width={24} height={24} />
          <li
            class="pb-4 test55 sm:text-xl text-lg [@media(max-width:371px)]:text-base [@media(max-width:341px)]:text-sm [@media(max-width:330px)]:text-xs"
          >
            <a href="mailto:info@stockholmsteelband.se"
              >info@stockholmsteelband.se</a
            >
          </li>
        </div>
        <!-- <div class="flex gap-2">
                    <PhoneIcon width={24} height={24}/> 
                    <li class="test55 pb-4 sm:text-xl text-lg  [@media(max-width:371px)]:text-base  [@media(max-width:314px)]:text-sm   [@media(max-width:300px)]:text-xs  "><a href="tel: +46723604748">+46 72-360 47 48</a></li>
                </div> -->
        <div class="flex justify-center">
          <li>
            <a
              class="items-center"
              target="”_blank”"
              href="https://www.facebook.com/stockholmsteelband/"
            >
              <img
                width="50px"
                src="/comany-logos/Facebook_Logo.png"
                alt="link to our Facebook"
                height="50px"
              />
            </a>
          </li>
          <li class="  ">
            <a
              class=" "
              target="”_blank”"
              href="https://www.instagram.com/stockholmsteelband/"
            >
              <img
                class="logo2"
                width="90px"
                src="/comany-logos/Instagram-Logo.png"
                alt="link to our Instagram"
                height="51px" 
              />
            </a>
          </li>
          <li class="flex justify-center items-center">
            <a
              class="flex justify-center items-center"
              target="”_blank”"
              href="https://www.youtube.com/@stockholmsteelband"
            >
              <img
                class="logo3"
                alt="link to our Youtube"
                src="/comany-logos/youtube.png"
                width="55px" 
                height="39px"
              />
            </a>
          </li>
        </div>
      </ul>
    </div>
    <div class=" w-1/2 hidden lg:pl-10 lg:justify-end lg:flex justify-center">
      <img
        width="297px"
        height="297px"
        alt="Steelband"
        class=" object-contain"
        src="/sliderImages/gruppbild regnbåge.jpg"
      />
    </div>
  </div>
</section>

<style>
  @media (max-width: 316px) {
    .test55 {
      font-size: 15px;
    }
  }
  @media (max-width: 294px) {
    .test55 {
      font-size: 14px;
    }
  }
</style>
