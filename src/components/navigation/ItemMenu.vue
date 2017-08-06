<template>
    <li>
        <a>{{label}}</a>
    </li>
</template>

<script>
export default {
    name: 'item-menu',
    props: {
        label: {
            type: String,
            required: true
        }
    }
};
</script>

<style lang="scss" scoped>
@import '../../assets/scss/_variables.scss';
@import '../../assets/scss/_mixins.scss';


li {
    // border: solid 1px yellow;
    color: white;
    display: inline;
    padding: 2rem;
    >a {
        text-transform: uppercase;
        font-size: $label-menu;
        cursor: pointer;
        @include simple-transition(200ms ease-out);
        position: relative;
        &:hover {
            color: $pink;
            &:after {
                width: 100%;
            }
        }
        &:after {
            position: absolute;
            content: '.';
            text-align: center;
            @include simple-transition(200ms ease-out);
            color: transparent;
            bottom: -.4rem;
            width: 0;
            left: 0;
            border-bottom: solid .1rem $pink;
        }
    }
}
</style>
