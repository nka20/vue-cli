<template>
<div>
<center>
<button class="btn-sm btn-primary" @click="diminuer">-</button>
<!--<p>{{count}}</p>-->
<count count :number="count"></count>
<button class="btn-sm btn-primary" @click="augmenter">+</button>
</center>
</div>
</template>
<script>
import count from "../components/TestView.vue"
export default{
    components:{
count, 
},
name:'TestView',
data() {
    return{
count:0
    };
},
 methods:{
    diminuer(){
        this.count-=1
    },
       augmenter(){
        this.count+=1
    }
}
}

</script>
<style>
</style>
