<script>
import PrimaryButton from "$lib/ui/PrimaryButton.svelte";

</script>
<div class="homeHeroSection">
  <h4>Award-winning custom designs and digital branding solutions</h4>
  <p class="body-2">With over 10 years in the industry, we are experienced in creating fully responsive websites, app design, and engaging brand experiences. Find out more about our services.</p>
  <PrimaryButton buttonColor={'#fff'} buttonText={"Learn More"}></PrimaryButton>
  <img class="hero-image" src="/assets/home/desktop/image-hero-phone.png" alt="Hero Phone" />
</div>

<style>
  h4 {
    color: #fff;
    text-align: center;
    font-weight: 400;
    margin-bottom: 16px;
  }
  p {
    color: #fff;
    text-align: center;
    margin-bottom: 24px;
  }
  .hero-image {
    position: absolute;
    top: 300px;
    left: 50%;
    transform: translateX(-50%);
    width: 170%;
  }
</style>