<script lang="ts">
  export let isMobile: boolean = true
</script>

<div class="topBarContainer">
  <a href="/" class="logoContainer">
    <img src="/assets/shared/desktop/logo-dark.png" alt="Logo">
  </a>
  {#if isMobile}
    <div class="hamburgerMenu">
      <img src="/assets/shared/mobile/icon-hamburger.svg" alt="Menu Icon">
    </div>
  {/if}
</div>