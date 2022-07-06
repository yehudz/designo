<script lang="ts">
  import { fly } from 'svelte/transition';
  import { mobileMenuVisibility } from '$lib/context/mobileMenuVisibility';
  export let toggleMenu: ()=> void
</script>

<div class="mobileMenuContainer">
  <div class="menuList">
    <a in:fly={{y: -50, duration: 550}} on:click={toggleMenu} href="/about">Our Company</a>
    <a in:fly={{y: -50, duration: 550, delay: 100}} on:click={toggleMenu} href="/locations">Locations</a>
    <a in:fly={{y: -50, duration: 550, delay: 200}} on:click={toggleMenu} href="/contact">Contact</a>
  </div>
  <div class="overlay"></div>
</div>