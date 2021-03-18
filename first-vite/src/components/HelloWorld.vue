<template>
        <h1>{{ msg }}</h1>
        <button @click="count++">count is: {{ count }}</button>
        <p>Edit <code>components/HelloWorld.vue</code> to test hot module replacement.</p>
        <div>你好啊ee5555e啊</div>
        <div>{{arr}}</div>
</template>

<script>
    export default {
        name: 'HelloWorld',
        props: {
            msg: String
        },
        data() {
            return {
                count: 0,
                arr: [1, 2, 3, 4],
            }
        },
        mounted() {
            setTimeout(() => {
                this.arr[2] = 'lsk';
                this.arr.length=3
            },2000)
        }
    }
</script>
