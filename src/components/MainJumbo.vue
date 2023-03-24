<script>
export default {
    name: 'MainJumbo'
}
</script>

<template>
    <section id="jumbo"></section>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;

    #jumbo {
        height: 400px;
        background-image: url('../assets/jumbotron.jpg');
        background-repeat: no-repeat;
        background-size: cover;
    }
</style>
