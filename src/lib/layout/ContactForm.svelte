<script lang="ts">
  import PrimaryButton from "$lib/ui/PrimaryButton.svelte";
import PrimaryInput from "$lib/ui/PrimaryInput.svelte";
import PrimaryTextField from "$lib/ui/PrimaryTextField.svelte";
</script>

<div class="contactFormContainer">
  <div class="content">
    <h4>Contact Us</h4>
    <p class="body-2">
      Ready to take it to the next level? Let’s talk about your project or idea and find out how we can help your business grow. If you are looking for unique digital experiences that’s relatable to your users, drop us a line.
    </p>
  </div>
  <div class="contactContent">
    <PrimaryInput placeholder="Name" type="text"/>
    <PrimaryInput placeholder="Email" type="email"/>
    <PrimaryInput placeholder="Phone" type="tel"/>
    <PrimaryTextField placeholder="Your Message"/>
    <br>
    <PrimaryButton buttonColor="white" buttonText="Submit">Submit</PrimaryButton>
    <br>
  </div>
</div>
