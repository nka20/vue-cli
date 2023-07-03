<template> <!-- grace au slot ceux qu'on ecrira ira au slot-->
<overlay @allan="$emit('close')"><h1>Ajouter employer comme {{donner}}</h1>

    <form>
        <label>Id: </label>
        <input type="text">
<br>
<br>
        <label>nom: </label>
        <input type="text">
<br>
<br>

        <label>prenom: </label>
        <input type="text">
<br>
<br>

        <label>age: </label>
        <input type="number">
<br>
<br>

            <label>genre: </label>
        <input type="text">
<br>
<br>

        <label>status: </label>
        <input type="text">
        
<br>
<br>
<br>
<br>
<br>
        <button style="color:white; padding:20px; background-color:red; margin-left:250px;">envoyer</button>
        <button @click="$emit('allan')" style="color:white; padding:20px; background-color:blue; margin-left:250px;">close</button>
        </form>
</overlay>
</template>
<script>
import Overlay from "./OverlayView.vue"
export default{
    props:["donner"],
    components:{
    Overlay,
},
name:'AddEmployee',
data() {
    return{

    }
}
}
</script>
<style>
 input{
	height:20px;
	border:1px solid green;
}
</style>
