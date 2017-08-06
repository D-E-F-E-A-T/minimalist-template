<template>
    <div>
        <text-image :image="MainBackground">
            ssss
        </text-image>
    </div>
</template>

<script>
import TextImage from '../text-image/TextImage';
import MainBackground from '../../assets/images/background-two.jpg';

export default {
    name: 'navigation',
    data() {
        return {
            MainBackground
        };
    },
    components: {
        TextImage
    }
};
</script>

<style lang="scss" scoped>

</style>
