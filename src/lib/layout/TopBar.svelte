<script lang="ts">
  import MobileMenu from "$lib/ui/MobileMenu.svelte"
	import { mobileMenuVisibility } from '$lib/context/mobileMenuVisibility';
  export let isMobile: boolean = true
  function toggleMenu() {
    mobileMenuVisibility.update(n=> n = !n)
    document.body.classList.toggle('noScroll'); 
  }
</script>
<div class="topBarContainer">
  <a href="/" class="logoContainer">
    <img src="/assets/shared/desktop/logo-dark.png" alt="Logo">
  </a>
  {#if isMobile}
    <div class="hamburgerMenu" on:click={toggleMenu}>
      <img src="/assets/shared/mobile/icon-hamburger.svg" alt="Menu Icon">
    </div>
  {/if}
</div>
{#if $mobileMenuVisibility}
  <MobileMenu />
{/if}