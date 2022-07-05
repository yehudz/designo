<script lang="ts">
  export let image: string
  export let title: string
  export let url: string
</script>

<div class="viewProjectCard" style={`background-image: url(${image})`}>
  <div class="title">{title}</div>
  <a href={url} class="viewProject">View Project <img src="assets/shared/desktop/icon-right-arrow.svg" alt=""></a>
</div>