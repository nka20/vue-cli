<template> <!-- grace au slot ceux qu'on ecrira ira au slot-->
<overlay @allan="$emit('close')">
			<form>
				<label>nom: </label>
				<input type="text" v-model="datam.nom">
<br>
<br>

				<label>prenom: </label>
				<input type="text" v-model="datam.prenom">
<br>
<br>

				<label>age: </label>
				<input type="text" v-model="datam.age">
<br>
<br>

					<label>genre: </label>
				<input type="text" v-model="datam.genre">
<br>
<br>

				<label>status: </label>
				<input type="text" v-model="datam.status">
				
<br>
<br>
<br>
<br>
<br>
				<button style="color:white; padding:20px; background-color:red; margin-left:250px;">envoyer</button>
				<button @click="$emit('close')" style="color:white,padding:20px; background-color:blue; margin-left:250px;">close</button>
				</form>
</overlay>
<!--<overlay>modifier {{data}}</overlay>-->
</template>
<script>
import Overlay from "./OverlayView.vue"
export default{
    props:["data"],
    components:{
    Overlay,
},
name:'ModifierView',
data() {
    return{
    datam:this.data
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
