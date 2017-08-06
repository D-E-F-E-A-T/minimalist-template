<template>
    <div class="container">
        <div class="dark-bg">
            <slot></slot>
        </div>
        <div class="img" :style="{'background-image':`url(${image})`}"></div>
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
    position: relative;
    max-height: 700px;
    overflow: hidden;
    > .img{
        width: 100%;
        height:750px;
        background-size: cover;
    }
    .dark-bg {
        position: absolute;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.5);
    }
}
</style>

