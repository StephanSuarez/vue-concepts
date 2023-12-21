<template>
  <!-- Methods -->
  <div>
    <p>getName: {{ getNamte("stephan") }}</p>
  </div>

  <!-- Events -->
  <div class="compo">
    <button @click="greeting">click</button>
  </div>
  <div class="compo">
    <button v-on:click="greeting">click</button>
  </div>
  <div class="compo">
    <button v-on:mousemove="greeting">click</button>
  </div>
  <div class="compo">
    <button v-on:dblclick="greeting">click</button>
  </div>
  <div class="compo">
    <button v-on:mouseleave="greeting">click</button>
  </div>

  <!-- Binding -->
  <div>
    <input type="text" placeholder="" v-model="valu">
  </div>
</template>

<script>
  export default {
    name: 'methodsParameters',
    data() {
      return{
        valu: "fa;lsdj fa;l"
      }
    },
    methods: {
      getNamte(name){
        return name
      },
      greeting(){
        return alert('hi');
      }
    }
  }
</script>

<style scoped>
  .compo{
    background: #fff;
  }
</style>