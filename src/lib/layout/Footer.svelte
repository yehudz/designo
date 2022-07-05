<script>
  import FooterContact from "$lib/components/FooterContact.svelte";
import FooterLogos from "$lib/components/FooterLogos.svelte";
import FooterMenu from "$lib/components/FooterMenu.svelte";
import FooterMessage from "$lib/components/FooterMessage.svelte";
</script>
<div class="footerContainer">
  <FooterMessage 
    title={"Let’s talk about your project"}
    text={"Ready to take it to the next level? Contact us today and find out how our expertise can help your business grow."}
  />
  <div class="footerContent">
    <div class="logoContainer">
      <img src="assets/shared/desktop/logo-light.png" alt="Footer logo">
    </div>
    <FooterMenu />
    <FooterContact title={"Designo Central Office"} text={"3886 Wellington Street Toronto, Ontario M9C 3J5"}/>
    <FooterContact title={"Contact Us (Central Office)"} text={`P : +1 253-863-8967 M : contact@designo.co`}/>
    <FooterLogos />
  </div>
</div>