<script context="module">
  import PageHeader from "$lib/components/PageHeader.svelte";
  import ShowCaseCard from "$lib/components/ShowCaseCard.svelte";
  import ViewProjectCard from "$lib/components/ViewProjectCard.svelte";
  import appdesignShowCaseData from "$lib/factories/app-design-show-case";
</script>
<PageHeader title={"App Design"} text={"Our mobile designs bring intuitive digital solutions to your customers right at their fingertips."}/>
<div class="showCase">
  {#each appdesignShowCaseData as item}
    <ShowCaseCard 
      image={item.image}
      title={item.title}
      subtitle={item.subtitle}
    />
  {/each}
  <div class="viewProjectsContainer">
    <ViewProjectCard 
      title={"Web Design"} 
      image={'/assets/home/mobile/image-web-design.jpg'}
      url={"web-design"}
    />
    <ViewProjectCard 
      title={"Graphic Design"} 
      image={'/assets/home/mobile/image-graphic-design.jpg'}
      url={"graphic-design"}
    />
  </div>
</div>