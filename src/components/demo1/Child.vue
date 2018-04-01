<template>
    <span>Hello {{message}}</span>
</template>
<script>
    export default {
        // 在 props 中声明获取父组件的数据通过 message 传过来
        props: ['message']
    }
</script>