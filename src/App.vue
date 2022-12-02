<template>
  <HelloWorldVue />
  <HelloOne/>
  <HelloOne/>
  <HelloOne/>

</template>

<script>
import HelloWorldVue from './components/HelloWorld.vue';
import HelloOne from'./components/heeloOne.vue'
export default {
  name: 'App',
  components: {
    HelloWorldVue,
    HelloOne
  }
}
</script>


