<script lang="ts">
  import LocationIllustationCard from '$lib/components/LocationIllustrationCard.svelte';
  import locationsData from '$lib/factories/locations-list-factory';
</script>
<div class="locationsContainer">
  {#each locationsData as location}
    <LocationIllustationCard name={location.name} illustration={location.ilustration} rotate={location.rotate}/>
  {/each}
</div>