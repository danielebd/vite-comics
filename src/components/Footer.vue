<script>
import FooterShop from './FooterShop.vue';
import FooterInfo from './FooterInfo.vue';
import FooterSub from './FooterSub.vue';

export default {
    name: 'Footer',
    components: {
        FooterInfo,
        FooterShop,
        FooterSub
    }
}
</script>

<template>
    <footer>
        <FooterShop></FooterShop>
        <FooterInfo></FooterInfo>
    </footer>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;

</style>