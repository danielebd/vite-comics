<script>
import MainJumbo from './MainJumbo.vue';
import MainComics from './MainComics.vue';
export default {
    name: 'Main',
    components: {
        MainJumbo,
        MainComics
    }
}
</script>

<template>
    <main>
        <MainJumbo></MainJumbo>
        <MainComics></MainComics>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;
    
    :deep(.title) {
        text-align: center;
    }
</style>