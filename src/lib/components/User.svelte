<script lang="ts">
    import { writable } from 'svelte/store';
    let ProfileLg : string = '../../images/ProfileLg.svg'
    let LogoIconLg : string = '../../images/LogoIconLg.png'
    let ExtLink : string = '../../images/ExtLink.svg'
    let isActive = writable(false);

    function toggleActive() {
        isActive.update(value => !value);
    }
</script>


<article class="flex gap-12 items-center" >
    <div class="flex flex-col justify-center items-center max-w-fit" >
        <img alt={'Profile picture'} src={ProfileLg} />
        <h1 class="font-bold text-2xl text-gray2 mx-auto w-32 text-center" >Krishna Kiran</h1>
    </div>

    <div>
        <p>Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of Engineering. I write hot-takes on building a business, shipping delightful products and accelerating product and career growth.
        </p>

         <button class={`${isActive ? 'shadow-bmd' : 'shadow-bms'} py-1.5 px-8 border border-[#4D4D4D] rounded-md flex items-center gap-2 hover:bg-[#0066FF] hover:shadow-md hover:shadow-[#003A91] hover:text-white hover:border-[#0066FF] mt-10 transition-all duration-300`} on:click={toggleActive}>
            {#if $isActive}
              Followed
            {:else}
              Follow
            {/if}
          </button>
    </div>

    <div class="flex flex-col items-end min-w-fit" >
        <img alt={'Profile'} src={LogoIconLg} />
        <h4 class="font-bold" > Duggup </h4>
        <p class="min-w-fit text-sm truncate text-gray1" > Co-Founder and CEO </p>

        <div class="flex justify-end items-center gap-4 mt-5 cursor-pointer" >
            <div class="flex items-center gap-1" >
                <p class=" text-linkGray text-sm min-w-fit hover:font-medium hover:text-blue" > My Website </p>
                <img src={ExtLink} alt="External Link" class='w-4 h-4' >
            </div>
            <div class="flex gap-1 hover:scale-110 transition-all duration-300" >
                <p class="w-1.5 h-1.5 bg-gray1 hover:bg-blue rounded-full" ></p>
                <p class="w-1.5 h-1.5 bg-gray1 hover:bg-blue rounded-full" ></p>
                <p class="w-1.5 h-1.5 bg-gray1 hover:bg-blue rounded-full" ></p>
            </div>
        </div>
    </div>
</article>