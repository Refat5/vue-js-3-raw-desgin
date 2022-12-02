<template>
    <div class="heading">
        <h1>Hello Home Component </h1>
        <h3>Hello Home Component </h3>
        <div class="center">
            <strong>Sum Of Two number {{10 + 32}}</strong>
            <h4>Length Of a String {{"Abdur Rahim Refat".length}}</h4>
            <h2>this is my mobile number {{(mobile=2332)}}</h2>

            Show my email from data<a href=""> {{email}}</a>
            show the function from data <p>{{myfunction()}}</p>

            <h2>Function with Parameter {{secondFunction('Hello Refat Your Second Function')}}</h2>
            
            <br>
            <br>
            <h4> My Friend Name</h4>
              <h5>My Name is {{myName()}}</h5>
              <h3> <h2> </h2> Friend {{getName('Fahad')}}</h3>
              <h3> <h2> </h2> Friend {{getName('Tanvir')}}</h3>



              <div>
                   <h3>Show my data from a Get data object </h3>
                   <p> {{getData().name}}</p>
                   <a href="">{{getData().email}}</a>
              </div>
        </div>

    </div>
</template>

<script>
export default{
    name:'HelloOne',
    data(){
        return{
            email : "Refat23@gmail.com",
            mobile: 32092,
            myfunction: function(){
                return "this is my function data"
            },
            secondFunction: function(value){
                return value
            },
        }
    },
    methods: {
        myName(){
           return " Abudr Rahim Refat"
        },
        getName(value){
            return  value
        },
        getData(){
                 return {
                      name: "Refat",
                      dpt: "Cse",
                      mobile: '0939043',
                      email: this.email
                 }
        }
    }
}

</script>

<style scoped>

.heading{
    text-align: center;
}
h2{
    color:green;
}
h3{
    color: gray;
}
</style>