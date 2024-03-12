<script>
  import FaChevronUp from "svelte-icons/fa/FaChevronUp.svelte";
import CardsContainer from "./CardsContainer.svelte";
  let LogoIconLg = '../../images/LogoIconLg.png';
  let BetterUp = '../../images/BetterUp.png';
</script>


<section class="mt-4 flex" >
<div>

    <div class="w-[60px] mb-14 pt-8" >
        <div class='h-[225px] relative w-[60px]' >
            <div class='flex gap-5 absolute top-[46%] -right-[9.5px]' >
                <p class='text-gray1 text-sm truncate' >Dec 2023</p>
                <div class='w-4 h-4 rounded-full bg-blue grid place-items-center'>
                    <p class='w-2 h-2 rounded-full bg-white' ></p>
                </div>
            </div>
        </div>
    </div>

    <!-- next one -->
    <div class="w-[60px] mb-10 " >
        <div class='h-[80px] relative w-[60px]' >
            <p class='w-4 h-4 absolute -right-[9px] bg-white text-borderGray -top-8' ><FaChevronUp/></p>
            <div class=' gap-3  flex' >
                <div class="flex flex-col items-end absolute -top-2 right-8 text-xs " >
                    <img alt={'Profile'} src={LogoIconLg} />
                    <h4 class="font-bold text-sm" > Duggup </h4>
                    <p class="min-w-fit truncate text-gray1" > San Francisco Bay Area </p>
                    <p class="min-w-fit truncate text-gray1" > Joined  </p>
                    <p class="min-w-fit truncate text-gray1" > Nov 2023 </p>
        
                </div>
                <div class='w-7 h-7 rounded-full grid place-items-center bg-blue absolute top-[46%] -right-[15px]'>
                    <p class='w-2 h-2 rounded-full bg-white' ></p>
                </div>            
            </div>
        </div>
    </div>
        <!-- next one -->

    <div class="w-[60px] mb-12 pt-8" >
        <div class='h-[225px] relative w-[60px]' >
            <div class='flex gap-5 absolute top-[46%] -right-[9.5px]' >
                <p class='text-gray1 text-sm truncate' >Dec 2023</p>
                <div class='w-4 h-4 rounded-full bg-blue grid place-items-center'>
                    <p class='w-2 h-2 rounded-full bg-white' ></p>
                </div>            
            </div>
        </div>
    </div>

    <!-- next one -->
    <div class="w-[60px]" >
        <div class='h-[80px] relative w-[60px] mb-40' >
            <p class='w-4 h-4 absolute -right-[9px] bg-white text-borderGray -top-8' ><FaChevronUp/></p>
            <div class='gap-3 flex' >
                <div class="flex flex-col items-end absolute -top-2 right-8 text-xs " >
                    <img alt={'Profile'} src={BetterUp} />
                    <h4 class="font-bold text-sm" > BetterUp </h4>
                    <p class="min-w-fit truncate text-gray1" > San Francisco Bay Area </p>
                    <p class="min-w-fit truncate text-gray1" > Joined  </p>
                    <p class="min-w-fit truncate text-gray1" > Sept 2022 </p>
        
                </div>
                <div class='w-7 h-7 rounded-full grid place-items-center bg-blue absolute top-[46%] -right-[15px]'>
                    <p class='w-2 h-2 rounded-full bg-white' ></p>
                </div>
            </div>
        </div>
    </div>
        <!-- next one -->

  
</div>


    <CardsContainer/>
</section>