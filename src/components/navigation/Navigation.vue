<template>
    <div>
        <text-image :image="MainBackground">
            <template>
                <navbar></navbar>
            </template>
        </text-image>
    </div>
</template>

<script>
import TextImage from '../text-image/TextImage';
import MainBackground from '../../assets/images/background.jpeg';
import Navbar from './Navbar';

export default {
    name: 'navigation',
    data() {
        return {
            MainBackground
        };
    },
    components: {
        TextImage,
        Navbar
    }
};
</script>

<style lang="scss" scoped>

</style>
