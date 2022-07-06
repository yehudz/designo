<script lang="ts">
  import PrimaryButton from "$lib/ui/PrimaryButton.svelte";
  import PrimaryTextField from "$lib/ui/PrimaryTextField.svelte";
  let nameValue: string
  let emailValue: string
  let telValue: number
  let validateName: boolean = false
  let validateEmail: boolean = false
  let validatePhone: boolean = false
  let formSubmitted: boolean = false
  function submitForm() {
    formSubmitted = true
    setTimeout(()=> {
      formSubmitted = false
    }, 3000)
    if (nameValue) validateName = true
    if (emailValue) validateEmail = true
    if (telValue) validatePhone = true

    let params = {
      nameValue,
      emailValue,
      telValue
    }
  }

</script>
<div class="contactFormContainer">
  <div class="content">
    <h4>Contact Us</h4>
    <p class="body-2">
      Ready to take it to the next level? Let’s talk about your project or idea and find out how we can help your business grow. If you are looking for unique digital experiences that’s relatable to your users, drop us a line.
    </p>
  </div>
  <div class="contactContent">
    <div class="inputContainer">
      {#if formSubmitted && !validateName}
        <label class="error" for="nameInput">Can't be empty</label><img src="assets/contact/desktop/icon-error.svg" alt="Error">
      {/if}    
      <input type="text" class="primaryInput" name="nameInput" placeholder="Name" bind:value={nameValue}/>
    </div>
    <div class="inputContainer">
      {#if formSubmitted && !validateEmail}
        <label class="error" for="emailInput">Can't be empty</label><img src="assets/contact/desktop/icon-error.svg" alt="Error">
      {/if}  
      <input type="email" class="primaryInput" name="emailInput" placeholder="Email" bind:value={emailValue}/> 
    </div>
    <div class="inputContainer">
      {#if formSubmitted && !validatePhone}
        <label class="error" for="phoneInput">Can't be empty</label><img src="assets/contact/desktop/icon-error.svg" alt="Error">
      {/if}    
      <input type="tel" class="primaryInput" name="phoneInput" placeholder="Phone" bind:value={telValue}/>
    </div>
    <div class="inputContainer">
      <PrimaryTextField placeholder="Your Message"/>
    </div>
    <br>
    <PrimaryButton 
      buttonColor="white" 
      buttonText="Submit"
      {submitForm}
    >Submit</PrimaryButton>
    <br>
  </div>
</div>
