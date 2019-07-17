<template>


        <button v-on:click="emit">{{message}}</button>
</template>

<script>
    import {Vue} from "vue";

    export default {
        name:"Button",
        data(){
            return {
                message: "hello world",
                appear: false
            }
        },

        methods: {
            reverseMessage: function() {
                this.message = this.message.split('').reverse().join('');
            },

            emit: function(){
                    this.$eventHub.$emit('openBox');
            }




        }


    }

    function emit(){
            this.$eventHub.$emit('openBox');
    }



</script>

<style>
    button{

        width: 100%;
        background-color: green;

    }
</style>
