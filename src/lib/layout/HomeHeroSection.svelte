<script>
import PrimaryButton from "$lib/ui/PrimaryButton.svelte";

</script>
<div class="homeHeroSection">
  <h4>Award-winning custom designs and digital branding solutions</h4>
  <p class="body-2">With over 10 years in the industry, we are experienced in creating fully responsive websites, app design, and engaging brand experiences. Find out more about our services.</p>
  <a href="/contact">
    <PrimaryButton buttonColor={'#fff'} buttonText={"Learn More"} submitForm={()=> {}}></PrimaryButton>
  </a>
  <img class="hero-image" src="/assets/home/desktop/image-hero-phone.png" alt="Hero Phone" />
</div>

<style lang="scss">
  h4 {
    font-size: 32px;
    color: #fff;
    text-align: center;
    font-weight: 400;
    margin-bottom: 16px;
    max-width: 316px;
    margin: 0 auto;
    margin-top: 48px;
    @media screen and (min-width: 736px) {
      font-size: 48px;
      max-width: 500px;
      line-height: 48px;
      margin-bottom: 24px;
    }
  }
  p {
    color: #fff;
    text-align: center;
    margin-bottom: 24px;
    @media screen and (min-width: 736px) {
      font-size: 16px;
      max-width: 455px;
      margin: 0 auto;
      margin-bottom: 48px;
    }
  }
  .hero-image {
    position: absolute;
    top: calc(50% + 325px);
    left: 50%;
    transform: translate(-50%, -50%);
  }
</style>