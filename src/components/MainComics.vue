<script>
export default {
    name: 'MainComics'
}
</script>

<template>
    <section class="container">

        <div class="container-comics-list">
            <h2 class="title-section">CURRENT SERIES</h2>
            <div class="comics-list"></div>
            <div class="button">
                <button>LOAD MORE</button>
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;

.container {
    background-color: #1c1c1c;
    color: white;

    .container-comics-list {
        max-width: $bigContainer;
        position: relative;
        margin: 0 auto;


        h2 {
            margin: 0;
            padding: 10px 30px;
            background-color: $primaryColorBlue;
            display: inline-block;
            position: absolute;
            top: -30px;
        }

        .comics-list {
            height: 650px;
        }

        .button {
            padding: 20px 0;
            

            button {
                margin: 0px auto;
                display: block;
                background-color: $primaryColorBlue;
                color: white;
                border: none;
                font-size: 20px;
                padding: 10px 50px;
                cursor: pointer;
            }
        }


    }
}
</style>