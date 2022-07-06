<script lang="ts">
  export let country: string
  export let title: string
  export let address: string
  export let contactTitle: string
  export let contactPhone: string
  export let contactEmail: string
  export let map: string
</script>

<div class="locationCard">
  <img src={map} alt={title}>
  <div class="content">
    <div class="country">{country}</div>
    <div class="textContent">
      <div class="title">{title}</div>
      <div class="address">{address}</div>
    </div>
    <div class="textContent">
      <div class="contactTitle">{contactTitle}</div>
      <div class="contactPhone">{contactPhone}</div>
      <div class="contactEmail">{contactEmail}</div>
    </div>
  </div>
</div>