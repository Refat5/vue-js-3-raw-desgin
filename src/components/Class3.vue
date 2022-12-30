<template>

<div>
    <h3>this is my input Class</h3>


    <center>
        <div class="card">
            <input type="text" placeholder="Enter Your name" v-model="email">
            <br>
            <br>
            <input type="number" placeholder="Enter the number" v-model="phone">
       <br>
       <br>
            <button type="button" v-on:click="getData()">Get Value</button>
        </div>
    
    </center>
</div>

<CheckBok/>
</template>

<script>
import CheckBok from './CheckBok.vue';
export default{
    name, 
    components:{
      CheckBok,
    },
    data(){
            return{
                email: null,
                phone:null,
            }
    },
    methods: {
         getData(){
            console.log(this.email, this.phone);

         }
    },
}
</script>