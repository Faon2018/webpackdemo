<template>
        <mt-header fixed :title="title" >
            <slot name="left">
                <mt-button icon="back" slot="left"></mt-button>
            </slot>
            <slot name="right">
                <!--此处的slot是组件header里的slot-->
                <mt-button  slot="right" @click="">登录|注册</mt-button>
            </slot>

        </mt-header>
</template>

<script>
    export default {
        name: "Head",
        props:{
            title:String
        }

    }
</script>

<style scoped>

</style>