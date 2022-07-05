<script lang="ts">
import PrimaryButton from "$lib/ui/PrimaryButton.svelte"

  export let title: string
  export let text: string
</script>

<div class="footerMessageContainer">
  <h4>{title}</h4>
  <p class="body-2">
    {text}
  </p>
  <PrimaryButton buttonText={"Get in touch"} buttonColor="white"></PrimaryButton>
</div>

<style lang="scss">
  .footerMessageContainer {
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 24px;
    margin-top: 72px;
    overflow: hidden;
    &::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      height: 100%;
      width: 100%;
      background-image: url('assets/home/desktop/bg-pattern-hero-home.svg');
      background-size: 100%;
      transform: rotate(90deg);
    }
    
    h4 {
      color: #fff;
      text-align: center;
      margin-bottom: 16px;
    }
    .body-2 {
      color: #fff;
      text-align: center;
      margin-bottom: 24px;
    }
  }
</style>