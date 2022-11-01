<script lang="ts">
  import Navbar from "./Components/Navbar/Navbar.svelte";
  import About from "./Components/About/About.svelte";
  import Footer from "./Components/Footer/Footer.svelte";
  import DATA from "./Data/data";
</script>

<main>
  <Navbar navlists={DATA.NAVBAR_DATA} header={DATA.HEADER} />

  <About aboutData={DATA.ABOUT_DATA} />

  <Footer />
</main>

<style>

</style>