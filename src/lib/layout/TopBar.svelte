<script lang="ts">
  export let isMobile: boolean = true
</script>

<div class="topBarContainer">
  <div class="logoContainer">
    <img src="/assets/shared/desktop/logo-dark.png" alt="Logo">
  </div>
  {#if isMobile}
    <div class="hamburgerMenu">
      <img src="/assets/shared/mobile/icon-hamburger.svg" alt="Menu Icon">
    </div>
  {/if}
</div>