<script>
    import PhoneIcon from '../icons/phone-call-icon.svelte'
    import EmailIcon from '../icons/Email-forward-icon.svelte'
</script>

<section id="Boka-oss" class="pb-20 mb-24 mt-14 outline rounded-2xl mx-auto max-w-4xl pb ">
    <h2 class="text-center pt-8 lg:py-14">Boka Oss</h2>
    <div class="lg:flex gap-8 flex px-24 ">
        
        <div class="basis-2/4 flex items-center justify-start lg:pt-0 lg:pb-4 pt-10" >
            <ul class=" p   pt-4">
                <div class="flex gap-2">
                    <PhoneIcon width={24} height={24}/> 
                    <li class="pb-4"><a>info@stockholmsteelband.se</a></li>
                </div>
                <div class="flex gap-2">
                    <EmailIcon width={24} height={24}/> 
                    <li class="pb-4"><a>+46 72-360 47 48</a></li>
                </div>
                <div class="flex">
                    <li>
                         <a class="items-center " target=”_blank”   href="https://www.facebook.com/stockholmsteelband/">
                                    <img width="50" src="\comany logos\Facebook_Logo_(2019).png.webp"/>
                        </a>
                     </li>
                    <li class="  "><a class=" " target=”_blank”   href="https://www.instagram.com/stockholmsteelband/">
                            <img class="logo2" width="90px" src="\comany logos\Instagram-Logo.png"/>
                        </a>
                    </li>
                    <li class="flex justify-center items-center"><a class="flex justify-center items-center" target=”_blank”   href="https://www.youtube.com/@stockholmsteelband">
                                <img class="logo3"  width="55" src="\comany logos\youtube.png"/>
                            </a>
                    </li>
                </div>
            </ul>
        </div>
        <div class=" basis-2/4  lg:pl-10 lg:justify-end lg:block flex  justify-center " >
                    <img  width="400" alt="Steelband" class=" object-contain"  src="\images\Image of people in steelband.png"/>
        </div>
    </div>
</section>

