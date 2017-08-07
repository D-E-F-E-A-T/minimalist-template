<template>
    <div class="container" :style="{'background-image':`url(${image})`}">
        <div class="dark-bg">
            <slot></slot>
        </div>
    </div>
</template>

<script>
export default {
    name: 'text-image',
    props: {
        image: {
            type: String,
            required: true
        }
    }
};
</script>

<style lang="scss" scoped>
.container {
    width: 100%;
    background-size: cover;
    height: 750px;
    .dark-bg {
        height:100%;
        width: 100%;
        background: rgba(0, 0, 0, 0.7);
    }
}
</style>

