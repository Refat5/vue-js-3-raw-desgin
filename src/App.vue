<template>
 <div class="center">

     <HelloOne/>
     <IfElse/>
     <!-- <Class3/> -->
 </div>


</template>

<script>

import HelloOne from'./components/heeloOne.vue';
import IfElse from './components/IfElse.vue';
// import Class3 from'./components/Class3.vue';
export default {
  name: 'App',
  components: {
    HelloOne,
    IfElse
    // Class3
  }
}
</script>


