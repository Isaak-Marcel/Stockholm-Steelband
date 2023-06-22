<script>
</script>

<section class="sectionReal" >
    <video muted autoplay playsinline disablepictureinpicture loop class="w-full object-cover absolute -z-10 min  ">
        <source src="/videos/IMG_6793.mov" />
       
    </video>
    
</section>

<div class="MainWrapper relative z-2">
    <div class="mx-auto text-center w-10/12 -mt-32 z-10 ">
        <h2 class="mx-auto pb-4">vi spelar steelnabd</h2>
        <p class="steelP">Stockholm Steelband är ett oljefatsband som har sin givna plats när det kommer till att sprida dansglädje och feststämning. Musiken består av karibiska rytmer så som calypso och soca, med en blandad repertoar av traditionella låtskatter från Trinidad and Tobago och arrangemang av kända hits. Vi spelar på festivaler och företagsevent, firmafester – små som stora, privata fester, bröllop, dop, födelsedagsfirande, lokala gatufester, folkparker och karnevaler till större event i Stadshuset, Pride och Polarprisutdelning. Vi spelar både lugnare mingelmusik och smittande, oemotståndlig dansmusik. I samarbete med uppdragsgivaren skräddarsyr vi våra spelningar för att anpassa oss till era önskemål och upplägg.</p> </div>
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
    height: 50%;
    background: linear-gradient(transparent, black);
    z-index: 1;
}

    video{
        height: 750px;
    }
    .sectionReal{
            height: 700px;
    }

    /* Adjust the screen width value as needed */
    @media (max-width: 768px) {
        video{
            height: 600px;
        }
        .sectionReal{
            height: 400px;
        }
    }

    @media (max-width: 576px) {
        video{
            height: 450px;
        }
        .sectionReal{
            height: 250px;
        }
    }
</style>