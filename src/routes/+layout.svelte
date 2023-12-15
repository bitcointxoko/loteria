<script>
    import "../app.css";
    import Header from "../components/Header.svelte"
  </script>
  
<div class="container relative flex flex-col max-w-[1800px] mx-auto w-full text-sm sm:text-base min-h-screen">
    <Header/>
    <slot />
</div>
    