<script lang="ts" context="module">
  import LocationCard from '$lib/components/LocationCard.svelte';
  import locations from '$lib/factories/location-hub-factory';
</script>

<div class="locationsContainer">
  {#each locations as location}
    <LocationCard
      map={location.map}
      country={location.country}
      title={location.title}
      address={location.address}
      contactTitle={location.contactTitle}
      contactPhone={location.contactPhone}
      contactEmail={location.contactEmail}
    />
  {/each}
</div>