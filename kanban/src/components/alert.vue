<template>
<div  @click="change" :class="classname">
    {{help}} {{message}}
</div> 
</template>


    <script>
    export default {
        name: "Alert",
        props: ['message'],
        data: function()
        {
            return{
                help: "besoin d'aide?",
                classname: "alert alert-primary"
               }
        },
        methods:{
            change: function()
            {
                if (this.classname === "alert alert-primary") {
                    this.classname = "alert alert-success"
                }
                else
                this.classname = "alert alert-primary"
            }

        }

    } 
    </script>

    <style lang="scss">
    div{
        height:10vh;
    }
    .alert{
        position: relative;
        padding:.75 rem 1.25 rem;
        margin-bottom: 1 rem;
        border: 1 px solid transparent;
        border-radius: .25 rem;
        text-align: center;
        cursor: pointer;
    }

    .alert-primary{
        color: #004085;
        background-color: #cce5ff;
    }
    .alert-success{
        color: white;
        background-color: chocolate;
    }
    </style>