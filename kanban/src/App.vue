<template>
    <div id="app">
        <h1>
            Webpack sla merde
        </h1>
        <alert></alert>
    </div>
</template>


<script>
import Alert from './components/alert.vue'
export default {
    name: "app",
    components:{
        Alert
        }
}
</script>

<style lang="scss">
$color : red;
h1{
    background-color: $color;
    width: 30vw;
    margin: auto;
    text-align: center;
}
</style>