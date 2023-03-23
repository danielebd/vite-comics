<script>
export default {
    name: 'Main'
}
</script>

<template>
    <main>
        <h1>Content goes here</h1>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;

main {
    background-color: #1c1c1c;
    color: white;
    font-size: 30px;
    padding: 55px 10px;

    h1 {
        max-width: $bigContainer;
        margin: 0 auto;
    }
}
</style>