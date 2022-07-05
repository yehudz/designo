<script context="module">
  import PageHeader from "$lib/components/PageHeader.svelte";
  import ShowCaseCard from "$lib/components/ShowCaseCard.svelte";
  import ViewProjectCard from "$lib/components/ViewProjectCard.svelte";
  import graphicdesignShowCaseData from "$lib/factories/graphic-design-show-case";
</script>
<PageHeader title={"Graphic Design"} text={"We deliver eye-catching branding materials that are tailored to meet your business objectives."}/>
<div class="showCase">
  {#each graphicdesignShowCaseData as item}
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
      title={"Web Design"} 
      image={'/assets/home/mobile/image-web-design.jpg'}
      url={"web-design"}
    />
  </div>
</div>