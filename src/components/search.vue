<template>
    <h1>
        <input v-model="search" class="search__input" placeholder="查点啥"/>
    </h1>
    <span>{{res}}</span>
</template>

<script>
    export default {
        name: 'search',
        data: () => ({search: '', res: ''}),
        watch: {
            search(){
                const res = [
                    '哎呀，查不到呢~',
                    '哎呀，没做好呢~',
                    '最漂亮的女人当然是兰兰',
                    '做这玩意儿哪有这么简单呀',
                    '今天看起来胖了哈哈哈',
                    '由粤哥强力驱动',
                    '雕猫目前4.91kg',
                    '一天到晚都在想些啥呢',
                    '怎么可能？',
                    '哦！我的老天爷啊',
                ]
                this.res = res[Math.floor(Math.random()*10)]
            }
        }
    };
</script>

<style scoped>
    .search__input {
        border-radius: 16px;
        padding: 8px 16px;
        font-size: 16px;
        outline: none;
        border: 1px solid #999;
    }
</style>