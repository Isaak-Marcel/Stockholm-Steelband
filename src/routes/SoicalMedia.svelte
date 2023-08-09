<script>
    import PhoneIcon from '../icons/phone-call-icon.svelte'
    import EmailIcon from '../icons/Email-forward-icon.svelte'
</script>

<section class="flex flex-col gap-10">
    
    <ul class="flex  lg:gap-10 gap-4 pt-6 items-end  [@media(max-width:469px)]:items-start justify-center logos">
        <li class="flex  "><a class="flex flex-col items-center " target=”_blank”   href="https://www.facebook.com/stockholmsteelband/">
            <div class="lg:w-12 lg:h-12 w-9 ">
                <img width="60" alt="link to our Facebook" src="\comany logos\Facebook_Logo_(2019).png.webp"/>
            </div>
            <span  class='soicalATag text-center'>Stockholm Steelband</span>
            </a>
        </li>
    
        <li class="flex  ">
            <a class="flex flex-col items-center " target=”_blank”   href="https://www.instagram.com/stockholmsteelband/">

                <div class="lg:w-12 lg:h-12 w-9 flex justify-center items-center" >
                    <img class="logo2" src="\comany logos\Instagram-Logo.png"/>
                </div>
                <span  class='text-center   soicalATag'>stockholmsteelband</span>
            </a>
        </li>
        <li class="flex items-center justify-center  "><a class="flex flex-col justify-center items-center " target=”_blank”   href="https://www.youtube.com/@stockholmsteelband">
            <div class="lg:w-12 lg:h-12 w-9 flex justify-center items-center">
                <img class="logo3" width="80" src="\comany logos\youtube.png"/>
            </div>
            <span class='soicalATag text-center'>Stockholm Steelband</span>
            </a> 
        </li>
    </ul>
    <ul class="sm:flex-row flex flex-col  self-center gap-4 sm:gap-20">
       <div class="flex gap-2">
           <EmailIcon width={24} height={24}/>
            <a href ="mailto:info@stockholmsteelband.se"><li style="padding: 0"  class="pb-4">info@stockholmsteelband.se</li></a>
       </div>
       <!-- <div class="flex gap-2">
            <PhoneIcon width={24} height={24}/>
            <a href="tel: +46723604748"><li cstyle="padding: 0"  lass="pb-4">+46 72-360 47 48</li></a>
       </div> -->
    </ul>
</section>
    

<style>
    .logo2{
        max-width: 200%;
    }
    .logo3{
        max-width: 124%;
    }
    ul li span{
            padding-top: 5px;
    }
</style>