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

li {
    // border: solid 1px yellow;
    color: white;
    display: inline;
    >a {
        text-transform: uppercase;
        font-size: $label-menu;
        padding: 2rem;
    }
}
</style>
