
<script>
	import FaPlus  from 'svelte-icons/fa/FaPlus.svelte';
  import FaChevronDown from 'svelte-icons/fa/FaChevronDown.svelte'
  let links = [
    { text: 'Home', url: '#' , icon: '../../images/HomeIcon.svg'},
    { text: 'Explore', url: '#', icon: '../../images/Icon.svg' },
    { text: 'Learn', url: '#', icon: '../../images/Story.svg' },
  ];

  let Logo = '../../images/Logo.svg';
  let Profile = '../../images/Profile.png';
</script>

<nav class="py-4 pr-2 border-b border-dotted border-borderGray flex items-center justify-between sticky top-0 left-0 w-[100%] bg-white" >
       
  
  <a href={'/'} >
    <img src={Logo} alt="Logo">
  </a>

    <div class="flex justify-center items-center gap-10 text-linkGray" >
        {#each links as link}
          <a  href={link.url} class="flex items-center gap-2 w-16" >
            <img src={link.icon} alt="Home Icon" class='w-6 h-6' >
            <p class='text-sm hover:font-medium' >{link.text}</p>
          </a>
        {/each}

        <button class="py-1.5 px-8 border border-[#4D4D4D] rounded-md shadow-bmd flex items-center gap-2" > 
          <p class='w-4 h-4 font-light border border-black rounded-sm' > <FaPlus/> </p> 
          Post 
        </button>

        <div class="flex items-center gap-3 text-linkGray cursor-pointer" >
          <img src={Profile} alt="Profile Pic" class='w-12 h-12 border border-[#4D4D4D] rounded-full' >
          <h2 class="font-medium"> Krishna Kiran </h2>
          <span class='w-4 h-4' ><FaChevronDown/></span>
        </div>
    </div>
</nav>

