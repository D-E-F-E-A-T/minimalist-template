<template>
    <div class="nav-container">
        <logo></logo>
        <ul class="menu">
            <item-menu label="About"></item-menu>
            <item-menu label="Services"></item-menu>
            <item-menu label="Princig"></item-menu>
            <item-menu label="Contact"></item-menu>
        </ul>
    </div>
</template>

<script>
import Logo from './Logo';
import ItemMenu from './ItemMenu';

export default {
    name: 'navbar',
    components: {
        Logo,
        ItemMenu
    }
};
</script>

<style lang="scss" scoped>
.nav-container {
    // border:solid 1px purple;
    display: flex;
    justify-content: center;
    padding: {
        left: 2rem;
        right: 2rem;
        top: 1rem;
        bottom: 1rem;
    }
    >.menu {
        display: flex;
        align-items: center;
        list-style: none;
        // border:solid 1px blue;
    }
}
</style>
