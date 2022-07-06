<script lang="ts">
  import { fade, fly } from 'svelte/transition';
  import { mobileMenuVisibility } from '$lib/context/mobileMenuVisibility';
  function navigate() {
    document.body.classList.toggle('noScroll');
    mobileMenuVisibility.update(n=> n = !n)
  }
</script>

<div class="mobileMenuContainer">
  <div class="menuList">
    <a in:fly={{y: -50, duration: 500}} on:click={navigate} href="/about">Our Company</a>
    <a in:fly={{y: -50, duration: 500, delay: 100}} on:click={navigate} href="/locations">Locations</a>
    <a in:fly={{y: -50, duration: 500, delay: 200}} on:click={navigate} href="/contact">Contact</a>
  </div>
  <div class="overlay"></div>
</div>