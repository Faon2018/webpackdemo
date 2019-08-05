<template>
    <div>
        <Head :title="title">
            <div slot="right"></div>
        </Head>
        <mt-field label="username" placeholder="Input username" v-model="username"></mt-field>
        <mt-field label="password" placeholder="Input password" type="password" v-modal="password"></mt-field>
        <mt-field label="number" placeholder="Input number" type="number" v-model="number"></mt-field>
        <mt-field label="captcha" v-model="captcha">
            <img src="../assets/img/vertity.png" height="45px" width="100px">
        </mt-field>
        <mt-button type="primary">登录|注册</mt-button>
    </div>

    
</template>

<script>
    import Head from '../components/common/Head'
    export default {
        name: "Login",
        data(){
            return {
                title:'登录注册'
            }
        },
        components:{
            Head
        }
    }
</script>

<style scoped>

</style>