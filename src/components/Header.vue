<script>
export default {
    name: 'HeaderVue',
}
</script>

<template>
    <header>
        <div id="logo">
            <img src="../assets/dc-logo.png" alt="dc-logo">
        </div>
        <div id="menu">
            <ul>
                <li>CHARACTERS</li>
                <li>COMICS</li>
                <li>MOVIES</li>
                <li>TV</li>
                <li>GAMES</li>
                <li>COLLECTIBLES</li>
                <li>VIDEOS</li>
                <li>FANS</li>
                <li>NEWS</li>
                <li>SHOP</li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;

header {
    max-width: $bigContainer;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;

    #logo {
        padding: 15px 0;
        width: 90px;
        
        img {
            width: 100%;
        }
    }

    #menu {
        ul {
            margin: 0;
            box-sizing: border-box;

            li {
                box-sizing: border-box;
                display: inline-block;
                padding: 50px 0px;
                margin: 0 15px;
                border: 4px solid $primaryColorBlue transparent;

                &:hover {
                    border-bottom: solid 4px $primaryColorBlue;
                }
            }
        }

    }
}
</style>