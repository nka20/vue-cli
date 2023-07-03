<template> <!-- grace au slot ceux qu'on ecrira ira au slot-->
<overlay @allan="$emit('close')">

<form action="" method="post">
    <label for="">heure du debut : </label>
    <input type="date" v-model="conger_debut">
    <br>
    <br>
    <label for="">heure de fin : </label>
    <input type="date" v-model="conger_fin">
    <br>
    <br>
    <br>
    <br>
    <button type="button" @click="ajouter">ajouter conger</button>
</form>

</overlay>
</template>
<script>
    import Overlay from "./OverlayView.vue"
export default{
  
    components:{
    Overlay,
},
methods:{
    ajouter(){

    }
},
name:'AddConger',
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
