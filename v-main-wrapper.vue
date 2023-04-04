<template>
    <div class="v-main-wrapper">
        <p>{{  title }}</p>
        <vCatalog/>
        <vCard/>
    </div>
</template>

<script>
import vCatalog from './v-catalog';
import vCard from './v-card';

export default{
name: 'v-main-wrapper',
components:{
    vCatalog,
    vCard
},
props:{},
data(){
    return {
        title: 'Main wrapper',
    }
},
computed: {
methods:{},
watch:{},


}

}
</script>

<style scoped>
.v-main-wrraper{
max-width: 900px;
margin: 0 auto;
}
</style>