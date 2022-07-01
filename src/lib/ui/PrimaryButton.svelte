<script lang="ts">
  export let buttonText: string = 'Learn More';
  export let buttonColor: string = 'white'
</script>

<button class={`primaryButton ${buttonColor}`}>{buttonText}</button>