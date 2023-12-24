<template>
  <div>
    <p>show component</p>
    <component :is="componentName"></component>
    <button v-on:click="changeComponent()">change component</button>
  </div>
</template>

<script>
  import componentA from './componets ej/componentA.vue';
  import componentB from './componets ej/componentB.vue';

  export default {
    name: 'dinamic-components',
    data() {
      return {
        componentName: 'componentA'
      }
    },
    methods: {
      changeComponent(){
        this.componentName = this.componentName === 'componentA' ? 'componentB' : 'componentA'; 
      }
    },
    components: {
      componentA, 
      componentB
    }
  }
</script>

