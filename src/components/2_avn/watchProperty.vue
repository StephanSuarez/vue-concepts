<template>
  <div>
    <p>{{ count }}</p>
    <button v-on:click="increase()">+</button>
    <button v-on:click="decrease()">-</button>
  </div>
</template>

<script>
  export default {
    name: 'watch-property',
    data() {
      return {
        count: 0
      }
    },
    methods: {
      increase(){
        this.count+= 1
      },
      decrease(){
        this.count-= 1
      }
    },
    watch: {
      count(currentCount){
        if(currentCount > 5){
          alert('max val: 5')
          this.count = 5  
        }
        if(currentCount < -5){
          alert('min val: -5')
          this.count = -5
        }
      }
    }
  }
</script>

<style></style>