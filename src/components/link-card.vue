<template>
    <div class="link-card" @click="onCardClick">
        <span>
             {{label}}
        </span>
    </div>
</template>

<script>
    export default {
        name: 'link-card',
        props: {
            label: {
                type: String,
                default: ''
            },
            url: {
                type: String,
                default: ''
            }
        },
        methods: {
            onCardClick() {
                window.open(this.url);
            }
        }
    };
</script>

<style scoped>
    .link-card {
        width: 72px;
        height: 72px;
        border-radius: 8px;
        border: 1px solid #999;
        align-items: center;
        justify-content: center;
        display: inline-flex;
        transition: 0.3s;
        cursor: pointer;
        font-size: 14px;
        margin: 8px;
    }

    .link-card:hover {
        box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    }
</style>