<template>
  <h1>Initial App Vue Js</h1>
  <p>There is a component</p>
  <div>
    <h3>Firts component</h3>
    <MyComponent />
  </div>
  <div>
    <h3>Component with Interpolation</h3>
    <MyInterpolation />
  </div>
  <div>
    <h3>Methods, Parameters, Events</h3>
    <methodsParameters />
  </div>
  <div>
    <h3>If Else Condition</h3>
    <IfElse />
  </div>
  <div>
    <h3>For Loop</h3>
    <ForLoop />
  </div>
  <div>
    <h3>html binding</h3>
    <htmlBinding />
  </div>
  <div>
    <h3>Dinamic Class</h3>
    <dinamicClass />
  </div>
  <div>
    <h3>Data child to father</h3>
    <childFatherVue />
  </div>
  <div>
    <h3>Computed Property</h3>
    <computedProperty :number="0" />
  </div>
  <div>
    <h3>Watch Property</h3>
    <watchProperty /> 
  </div>
  <div>
    <h3 style="background-color: brown;">SLOTS</h3>
    <h3>Basic Slot</h3>
    <basicSlot>
      <p>M a slot and I take a property in app.vue: {{ slot }}</p>
    </basicSlot>
  </div>
  <div>
    <h3>Nominal Slot</h3>
    <nominalSlot>
      <template v-slot:section>
        <p>section one</p>
      </template>
      <template v-slot: section-two>
        <p>section two</p>
      </template>
    </nominalSlot>
  </div>
  <div>
    <h3>Dinamic Component</h3>
    <dinamic-component />
  </div>
</template>

<script>
import MyComponent from './components/MyComponent.vue';
import MyInterpolation from './components/interpolation.vue';
import methodsParameters from './components/MethodsParameters.vue';
import IfElse from './components/IfElse.vue';
import ForLoop from './components/ForLoop.vue';
import htmlBinding from './components/htmlBinding.vue';
import dinamicClass from './components/dinamicClass.vue';
import childFatherVue from './components/childFather.vue';
import computedProperty from './components/2_avn/computedProperty.vue';
import watchProperty from './components/2_avn/watchProperty.vue';
import basicSlot from './components/2_avn/slotBasic.vue';
import nominalSlot from './components/2_avn/slotNominal.vue';
import dinamicComponent from './components/2_avn/dinamicComponents.vue';

export default {
  name: 'App',
  data() {
    return {
      slot: "slot"
    }
  },
  components: {
    MyComponent,
    MyInterpolation,
    methodsParameters,
    IfElse,
    ForLoop,
    htmlBinding,
    dinamicClass,
    childFatherVue,
    computedProperty,
    watchProperty,
    basicSlot,
    nominalSlot,
    dinamicComponent
  }
}
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
  h3{
    background: #797c1c;
    color: #fff;
    padding: 10px 0;
  }
  .compo{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 50px;
    background: #2c3e50;
  }
</style>
