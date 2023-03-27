<script>
import { stringifyExpression } from '@vue/compiler-core';


export default {
    name: 'comicsBox',
    props: {
        img: String,
        series: String
    }
}
</script>

<template>
    <div>
        <div class="comic">
            <img :src="img" alt="#">
        </div>
        <div class="title">{{ series }}</div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;


</style>