<script lang="ts">
  export let image: string
  export let title: string
  export let text: string
  export let rotate: string
</script>

<div class="infomertialContainer">
  <div class="infomertialImageContainer">
    <img class={`bg ${rotate}`} src="assets/home/desktop/bg-pattern-hero-home.svg" alt={title}>
    <img class="img" src={image} alt={title}>
  </div>
  <div class="textContent">
    <h3>{title}</h3>
    <p class="body-2">{text}</p>
  </div>
</div>