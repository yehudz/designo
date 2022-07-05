<script lang="ts">
  import LocationCard from '$lib/components/LocationCard.svelte';
  import locationsData from '$lib/factories/locations-factory';
</script>
<div class="locationsContainer">
  {#each locationsData as location}
    <LocationCard name={location.name} illustration={location.ilustration} rotate={location.rotate}/>
  {/each}
</div>