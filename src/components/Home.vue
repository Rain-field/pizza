<template>
    <div>
        <h1>Home</h1>
        <button @click="goToMenu" class="btn btn-success">Go To Menu</button>
    </div>
</template>

<script>
export default {
    methods: {
        goToMenu(){
        // 跳转到上一次浏览的页面
        // this.$router.go(-1);

        // 跳转到指定的地址(菜单)
        // this.$router.replace('/menu');

        // 跳转到指定路由名字(name)下
        // this.$router.replace({name:'menuLink'});

        // 通过push压栈进行跳转(更常用)
        // this.$router.push('/menu');
        this.$router.push({name:'menuLink'});
        }
    }
}
</script>