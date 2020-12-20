<template>
    <div @click="$emit('click-fn')">
        <h1>Hello {{ name }} 😁</h1>
    </div>
</template>

<script>
    export default {
        name: 'HelloWorld',
        props: {
            name: String,
        },
        methods:{
            clickFn(){
                console.log('Click In HelloWorld')
            }
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
