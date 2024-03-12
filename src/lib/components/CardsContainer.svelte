<script lang="ts">
    import Card from './Card.svelte';
  
    let imgSrc0: string = '../../images/Image0.png';
    let imgSrc1: string = '../../images/Image1.png';
    let imgSrc2: string = '../../images/Image2.png';
    let imgSrc3: string = '../../images/Image3.png';

    let card0Text : string = 'No amount of technology can convert a bad story into a good story.'
    let card1Text : string = "Most people don't have original ideas. Here is how Sam Altman pushes himself to have unpopular ideas."
    let card2Text : string = `Startup Lesson I am reflecting. Don't build for the "average person".`
    let card3Text : string = `Your biggest regrets at 80 will be acts of omission.`


  </script>

  <section class="flex flex-col gap-16 max-w-fit border-l-2 border-dotted border-borderGray p-8" >

    <div class="flex gap-10" >
        <Card text={card0Text} imgSrc={imgSrc0} />
        <Card text={card1Text} imgSrc={imgSrc1} />

    </div>

    <div class="  p-4 rounded-xl shadow-sm shadow-[#DBE5F5]" >
        <h2 class="font-bold" > Co-Founder and CEO </h2>
        <div class="flex items-center gap-1 text-sm text-gray1" > <p> Full time </p>  <span class="w-0.5 h-0.5 bg-gray1 inline-block rounded-full" >  </span> <p> Remote </p> </div>

    </div>


    <div class="flex gap-10" >
        <Card text={card2Text} imgSrc={imgSrc2} />
        <Card text={card3Text} imgSrc={imgSrc3} />

    </div>


    <div class=" p-4 rounded-xl shadow-sm shadow-[#DBE5F5]" >
        <h2 class="font-bold" > VP Engineering </h2>
        <div class="text-sm text-gray1" > <p> Full-time </p> </div>

    </div>


      
    </section>