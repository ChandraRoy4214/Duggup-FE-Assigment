<script lang="ts">

    let Profile : string = '../../images/Profile.png'
    let LogoIconLg : string = '../../images/LogoIconLg.png'
  
  </script>


<article class="flex gap-12 items-center" >
    <div class="flex flex-col justify-center items-center max-w-fit" >
        <img alt={'Profile'} src={Profile} />
        <h1 class="font-bold text-2xl text-gray2 mx-auto w-32 text-center" >Krishna Kiran</h1>
    </div>

    <div>
        <p>Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of Engineering. I write hot-takes on building a business, shipping delightful products and accelerating product and career growth.

        </p>

        <button class="py-1.5 px-8 border border-[#4D4D4D] rounded-md shadow-bm flex items-center gap-2 hover:bg-[#0066FF] hover:shadow-md hover:shadow-[#003A91] hover:text-white hover:border-[#0066FF] mt-10 " > 
            Follow
         </button>
    </div>

    <div class="flex flex-col items-end" >
        <img alt={'Profile'} src={LogoIconLg} />
        <h4 class="font-bold" > Duggup </h4>
        <p class="min-w-fit truncate" > Co-Founder and CEO </p>

        <p class="mt-7" > My Website </p>
    </div>
</article>