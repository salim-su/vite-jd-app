<template>
    <div class="box"></div>
</template>

<script lang="ts">
    import {defineComponent, ref} from 'vue'

    export default defineComponent({
        name: 'HelloWorld',
        props: {
            msg: {
                type: String,
                required: true
            }
        },
        setup: () => {
            const count = ref(0)
            return {count}
        }
    })
</script>

<style lang="scss" scoped>
    a {
        color: #42b983;
    }

    label {
        margin: 0 0.5em;
        font-weight: bold;
    }

    code {
        background-color: #eee;
        padding: 2px 4px;
        border-radius: 4px;
        color: #304455;
    }

    .box {
        width: 100px;
        height: 100px;
        background-color: #2c3e50;
    }
</style>
