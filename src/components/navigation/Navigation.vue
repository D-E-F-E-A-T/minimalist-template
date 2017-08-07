<template>
    <div>
        <text-image :image="MainBackground">
            <template>
                <navbar></navbar>
                <text-banner></text-banner>
            </template>
        </text-image>
    </div>
</template>

<script>
import TextImage from '../text-image/TextImage';
import MainBackground from '../../assets/images/background.jpeg';
import Navbar from './Navbar';
import TextBanner from './TextBanner';

export default {
    name: 'navigation',
    data() {
        return {
            MainBackground
        };
    },
    components: {
        TextImage,
        Navbar,
        TextBanner
    }
};
</script>

<style lang="scss" scoped>

</style>
