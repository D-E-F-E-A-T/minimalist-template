<template>
    <div>
        <img :src="Logo">
    </div>
</template>

<script>
import Logo from '../../assets/images/logo.png';

export default {
    name: 'logo',
    data() {
        return {
            Logo
        };
    }
};
</script>

<style lang="scss" scoped>
div{
    // border:solid 1px red;
}
</style>
