<script lang="ts">
  import PrimaryButton from "$lib/ui/PrimaryButton.svelte"

  export let name: string
  export let illustration: string
  export let rotate: string
</script>

<div class="locationIllustationCard">
  <div class="illustration">
    <img src={illustration} alt={`Illustration of ${name}`}>
    <img src="assets/home/desktop/bg-pattern-hero-home.svg" class={`circle ${rotate}`} alt="background"/>
  </div>
  <div class="name">{name}</div>
  <a href="/locations">
    <PrimaryButton buttonColor="peach" buttonText="See location" submitForm={()=> {}}></PrimaryButton>
  </a>
</div>