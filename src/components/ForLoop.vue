<template>
  <div>
    <p>{{ data1 }}</p>
    <p>{{ data2 }}</p>
    <hr>
    <ul v-for="index in data1" :key="index">
      <li>
        {{index}}
      </li>
    </ul>
  </div>
  <div>
    <h3>Child Component and props</h3>
    <ForLoopChild msg="data2"/>
  </div>
  <div>
    <h3>Child Component and props</h3>
    <ForLoopChild :objData="data2['b']" />
  </div>
</template>

<script>
import ForLoopChild from './ForLoopChild.vue';
  
export default{
  name: "ForLoop",
  data() {
    return {
      data1: [1,2,3,{a:1}],
      data2: {'a':2, 'b': [1, 3]}
    }
  },
  components: {
    ForLoopChild
  }
}
</script>

<style>
</style>