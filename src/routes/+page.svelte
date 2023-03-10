<script>
  import '../app.css';
  import Contact from '../Components/Contact.svelte';
  import Hero from '../Components/Hero.svelte';
  import Projects from '../Components/Projects.svelte';
  import Specialities from '../Components/Specialities.svelte';
  import TopNav from '../Components/TopNav.svelte';
</script>

<svelte:head>
  <title>Salman</title>
</svelte:head>
<div class="App">
  <TopNav />
  <Hero />
  <Projects />
  <Specialities />
  <Contact />
</div>
