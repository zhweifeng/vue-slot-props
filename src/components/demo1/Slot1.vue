<template>
    <div class="app">
        <!-- message 定义在子组件的 props 中 -->
        <child :message="name"></child>
    </div>
</template>
<script>
    import Child from './Child.vue';
    export default {
        components: {
            Child
        },
        data() {
            return {
                name: 'linxin'
            }
        }
    }
</script>