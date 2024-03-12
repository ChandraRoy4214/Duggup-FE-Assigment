<script>
    import Nav from "$lib/components/Nav.svelte";
    import Home from "$lib/components/Home.svelte";
    import User from "$lib/components/User.svelte";
</script>


<main class="lg:max-w-[85vw] mx-auto text-darkGray" > 
    <Nav/>
    <section class="mt-12 max-w-[1120px] mx-auto" >
        <User/>
        <Home/>
    </section>
 </main>