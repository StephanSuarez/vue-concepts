<template>
  <p>
    {{msg}}  
  </p>
  <p>
    {{objData}}
  </p>
</template>

<script>
export default{
  name: "ChildComponent",
  props:{
    msg: String,
    objData: Array
  }
}
</script>

<style></style>