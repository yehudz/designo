<script context="module">
  import PageHeader from "$lib/components/PageHeader.svelte";
  import ShowCaseCard from "$lib/components/ShowCaseCard.svelte";
  import ViewProjectCard from "$lib/components/ViewProjectCard.svelte";
  import webdesignShowCaseData from "$lib/factories/web-design-show-case";
</script>
<PageHeader title={"Web Design"} text={"We build websites that serve as powerful marketing tools and bring memorable brand experiences."}/>
<div class="showCase">
  {#each webdesignShowCaseData as item}
    <ShowCaseCard 
      image={item.image}
      title={item.title}
      subtitle={item.subtitle}
    />
  {/each}
  <div class="viewProjectsContainer">
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
</div>