
<script>
import FaPlus from 'svelte-icons/fa/FaPlus.svelte'
  let links = [
    { text: 'Home', url: '#' },
    { text: 'Explore', url: '#' },
    { text: 'Learn', url: '#' },
  ];

  let Logo = '../../images/LogoIconSm.png';
  let Profile = '../../images/Profile.png';


</script>

<nav class=" py-2 pb-3 pr-2 border-b border-dotted border-borderGray flex items-center justify-between" >

<div class='flex items-center gap-1'>

<div>
<img src={Logo} alt="Description of the image">
</div>

<p class='font-semibold text-[#333333]' > duggup </p>
</div>

<div class="flex justify-center items-center gap-10" >
{#each links as link}
<div class="flex items-center gap-2" >
<p class='w-4 h-4 rounded-full bg-black' ></p>
<a href={link.url}>{link.text}</a>
</div>
{/each}

<button class="py-1.5 px-8 border border-[#4D4D4D] rounded-md shadow-bm flex items-center gap-2" > <p class='w-4 h-4 font-light border border-black rounded-sm' > <FaPlus/> </p> Post </button>

<div class="flex items-center gap-3" >
<img src={Profile} alt="Profile Pic" class='w-12 h-12 border border-[#4D4D4D] rounded-full' >

<h2 class="font-semibold"> Krishna Kiran </h2>
</div>
</div>


</nav>

