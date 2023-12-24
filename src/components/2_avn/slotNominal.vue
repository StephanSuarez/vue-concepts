<template>
  <div>
    <h6>Nominal Slot</h6>
    <slot name="section"></slot>
    <slot name="section-two">
      <h6>section-two</h6>
    </slot>
  </div>
</template>

<script>
  export default{
    name: 'nominal-slot'
  }
</script>
<style></style>