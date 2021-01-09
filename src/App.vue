<template>
    <logo msg="Hello Vue 3.0 + Vite"/>
    <search></search>
    <link-card label="画图用的" url="//www.draw.io"></link-card>
    <link-card label="粤哥博客" url="//streakingman.github.io"></link-card>
    <link-card label="晋江" url="//http://my.jjwxc.net/"></link-card>
</template>

<script>
    import Logo from './components/logo.vue';
    import Search from './components/search.vue';
    import LinkCard from './components/link-card.vue';

    export default {
        name: 'App',
        components: {
            LinkCard,
            Search,
            Logo
        }
    };
</script>

<style>

</style>
