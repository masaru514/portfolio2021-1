<script>
  import Tailwindcss from "./Tailwindcss.svelte";
  import Mainvisual from "../components/Mainvisual.svelte";
  import Feature from "../components/Feature.svelte";
  import Skills from "../components/Skills.svelte";
  import About from "../components/About.svelte";

  export let name;

  const h1 = "images/h1-text.svg";
</script>

<svelte:head>
  <link href="https://fonts.googleapis.com/css?family=Inter" rel="stylesheet" />
  <link
    href="https://fonts.googleapis.com/css2?family=Inter:wght@800&display=swap"
    rel="stylesheet"
  />
</svelte:head>

<Tailwindcss />
<header class="grid grid-cols-2 h-20 items-center">
  <h1 class="text-center text-2xl">
    <img class="mx-auto" src={h1} alt="Masaru Portfolio" />
  </h1>
  <nav>
    <ul class="lists w-80 mx-auto">
      <li><a class="block text-center" href="#about">ABOUT</a></li>
      <li><a class="block text-center" href="">CONTACT</a></li>
    </ul>
  </nav>
</header>
<main>
  <Mainvisual />
  <Feature />
  <Skills />
  <About />
</main>

<style lang="scss">
  .lists {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
  }
  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
