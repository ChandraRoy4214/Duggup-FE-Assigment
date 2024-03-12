<script lang="ts">
    export let imgSrc: string;
    export let text : string;
  </script>
  

  <article class="border border-[#D0D5DD] rounded-xl max-w-[344px]" >

    <img src={imgSrc} alt='card hero' class="rounded-t-xl" />

    <div class="p-5" >
        <p class=" line-clamp-2 h-12 overflow-hidden" >{text}</p>
    </div>
 
   
  </article>