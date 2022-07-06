<script lang="ts">
  import MobileMenu from "$lib/ui/MobileMenu.svelte"
	import { mobileMenuVisibility } from '$lib/context/mobileMenuVisibility';
  export let isMobile: boolean = true
  let imageSrc = "/assets/shared/mobile/icon-hamburger.svg"
  function toggleMenu() {
    mobileMenuVisibility.update(n=> n = !n)
    if ($mobileMenuVisibility) imageSrc = "/assets/shared/mobile/icon-close.svg"
    else imageSrc = "/assets/shared/mobile/icon-hamburger.svg"
    document.body.classList.toggle('noScroll'); 
  }
  console.log(imageSrc)
</script>
<div class="topBarContainer">
  <a href="/" class="logoContainer">
    <img src="/assets/shared/desktop/logo-dark.png" alt="Logo">
  </a>
  {#if isMobile}
    <div class="hamburgerMenu" on:click={toggleMenu}>
      <img src={imageSrc} alt="Menu Icon">
    </div>
  {/if}
</div>
{#if $mobileMenuVisibility}
  <MobileMenu {toggleMenu}/>
{/if}