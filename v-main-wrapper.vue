<template>
<div class="v-main-wrapper">
    <p>{{title}}</p>
    <v-catalog />
    <v-cart />


</div>

</template>

<script>
import Vcatalog from './components/v-catalog';
import Vcart from './v-cart';
  export default{
    name: 'v-main-wrapper',
    components: {
        vCatalog,
        vCart
    },
    props:{},
    data() {
    return{
    title: 'Main Wrapper'
        }
    },
    computed: {},
    methods: {},
    watch: {},
    mounted() {
        console.log('Hello i am alive!')
    }



}


</script>

<style>
.v-main-wrapper{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    max-width: 900px;
    margin: 0 auto;

}
</style>