<template>
    <div class="app">
        <!-- hide 为自定义事件，名字可以自己随便起，不能有大写字母，可以使用短横线 -->
        <!-- @hide 监听子组件触发 hide 事件，则会执行 hideDialog 方法 -->
        <dialog1 :is-show="show" @hide="hideDialog"></dialog1>
        <button @click="showDialog">显示弹框</button>
    </div>
</template>
<script>
    import dialog1 from './dialog.vue';
    export default {
        components: { dialog1 },
        data() {
            return {
                show: false
            }
        },
        methods: {
            showDialog() {
                this.show = true;
            },
            hideDialog() {
                this.show = false;
            }
        }
    }
</script>