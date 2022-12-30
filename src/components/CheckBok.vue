<template>
    
    <div style="text-align:center">
        <h3>this is my check box class</h3>
        <center>

             <h6>Programming Language</h6>
             <label for="php">Php </label>
             <input type="checkbox" id="php" value="php" v-model="programming_language">
            <br><br>
             <label for="javascript">Java Script </label>
             <input type="checkbox" id="javascript" value="javascript"  v-model="programming_language">
             <br><br>
             <label for="node">Node </label>
             <input type="checkbox" id="node" value="node"  v-model="programming_language">
             <br><br>
             <strong>Selected Programming Language : {{ programming_language }}</strong>


             <h3>What is your Age ?</h3>
             <label for="23">23</label>
             <input type="radio" value="23" name="age" v-model="age" id="23">

             <label for="24">24</label>
             <input type="radio" value="24" name="age" v-model="age" id="24">

             <label for="25">25</label>
             <input type="radio" value="25" name="age" v-model="age" id="25">
             <strong>Selected Programming Language : {{ age }}</strong>

        </center>
    </div>
</template>

<script>

export default{
    name,
    data(){
        return{
            programming_language: [ ],
            age: null
        }
    }
}
</script>