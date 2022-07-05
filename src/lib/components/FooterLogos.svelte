<script lang="ts">
  let icons = [
    '/assets/shared/desktop/icon-facebook.svg',
    '/assets/shared/desktop/icon-youtube.svg',
    '/assets/shared/desktop/icon-twitter.svg',
    '/assets/shared/desktop/icon-pinterest.svg',
    '/assets/shared/desktop/icon-instagram.svg',
  ]
</script>

<div class="footerLogos">
  {#each icons as icon}
    <img src={icon} alt="">
  {/each}
</div>