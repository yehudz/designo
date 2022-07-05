<script lang="ts">
  export let image: string
  export let title: string
  export let subtitle: string
</script>

<div class="showCaseCard">
  <img src={image} alt={title}>
  <div class="cardContent">
    <div class="title">{title}</div>
    <div class="subtitle">{subtitle}</div>
  </div>
</div>