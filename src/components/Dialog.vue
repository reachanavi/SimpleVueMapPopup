<template>
    <div id="main">

        <dialog-drag id="dialog-1">
            <div @click="test('hello flood response team')" id="dialogDiv">
                <p>Map would go here.</p><br>
                <p>Use the lock emoji to lock this window in place.</p>
            </div>
        </dialog-drag>

    </div>
</template>

<script>

    import DialogDrag from '../../node_modules/vue-dialog-drag';
    export default {
        name: 'Dialog',
        components: {
            DialogDrag
        },
        data:{
            appear: false
        },
        props: {
            message: String
        },
        created() {
            // this.$eventHub.$on('openBox', this.makeAppear);

        },

        methods: {
            test: function(message) {
                alert(message)
                console.log(message)
            },
            // makeAppear: function() {
            //     let x = document.getElementById("dialog-1");
            //     if (x.style.display === "none") {
            //         x.style.display = "block";
            //     } else {
            //         x.style.display = "none";
            //     }
            // },


        }
    }
</script>

<style src="vue-dialog-drag/dist/vue-dialog-drag.css">

</style>

<style>
    dialog-drag{
        z-index: 401;
    }
    #dialogDiv{
        z-index: 401;
    }
    p{
        z-index: 401;
    }

</style>