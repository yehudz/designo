<script context="module">
  import Footer from '$lib/layout/Footer.svelte';
  import TopBar from '$lib/layout/TopBar.svelte';
  import '../style/app.scss'
</script>
<main>
  <TopBar />
  <slot></slot>
  <Footer />
</main>