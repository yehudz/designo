<script>
  import ViewProjectCard from "$lib/components/ViewProjectCard.svelte";
</script>

<div class="viewProjectsContainer">
  <ViewProjectCard 
    title={"Web Design"} 
    image={'/assets/home/mobile/image-web-design.jpg'}
    url={"web-design"}
  />
  <ViewProjectCard 
    title={"App Design"} 
    image={'/assets/home/mobile/image-app-design.jpg'}
    url={"app-design"}
  />
  <ViewProjectCard 
    title={"Graphic Design"} 
    image={'/assets/home/mobile/image-graphic-design.jpg'}
    url={"graphic-design"}
  />
</div>