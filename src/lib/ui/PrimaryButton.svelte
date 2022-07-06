<script lang="ts">
  export let buttonText: string = 'Learn More';
  export let buttonColor: string = 'white'
  export let submitForm: ()=> void
</script>

<button class={`primaryButton ${buttonColor}`} on:click={submitForm}>{buttonText}</button>