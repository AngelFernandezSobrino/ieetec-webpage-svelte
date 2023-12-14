<script lang="ts">

  import svelteLogo from './assets/svelte.svg'
  import Content from './Content.svelte';
  import Footer from './Footer.svelte';
  import Header from './Header.svelte';
  import Counter from './lib/Counter.svelte'

</script>

<main>
  <Header />
  <Content />
  <div id="main-layout-spacer"></div>
  <Footer />
</main>

<style>
  main {
    display: flex;
    flex-direction: column;
    height: 100vh;
  }

  #main-layout-spacer {
    flex-grow: 1;
  }
</style>