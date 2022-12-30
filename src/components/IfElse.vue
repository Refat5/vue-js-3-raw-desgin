<template>
    <div>
        <center> Today we learn about IF else in vue </center>


          <h4 v-if="show">This is True That's why show this </h4>
          <h2 v-else> This is Else Condition</h2>

          <button  v-on:click="show=!show">Toogle Button</button>

    </div>
</template>

<script>

export default{

       data(){
        return{
               show: true
        }

       },
 
}
</script>

<style scoped>
h4{
    color: rgb(28, 89, 168);
}
h2{
    color: darkmagenta;
}

</style>