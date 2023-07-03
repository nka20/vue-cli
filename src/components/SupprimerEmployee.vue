<template> <!-- grace au slot ceux qu'on ecrira ira au slot-->
<overlay @close="$emit('close')">delete {{employeProps}}

</overlay>

</template>
<script>
import Overlay from "./OverlayView.vue"
export default{
    props:["employeProps"],
    name:'SupprimerEmployee',
    components:{
    Overlay,
},
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
