<script>
import comicsBox from './comicsBox.vue';
export default {
    name: 'MainComics',
    components: {
        comicsBox
    },
    data() {
        return {
            comicsList: [
                {
                    thumb: "https://picsum.photos/id/220/200/200",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "https://picsum.photos/id/237/200/200",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "https://picsum.photos/id/236/200/200",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "https://picsum.photos/id/239/200/200",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "https://picsum.photos/id/238/200/200",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "https://picsum.photos/id/235/200/200",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "https://picsum.photos/id/234/200/200",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://picsum.photos/id/233/200/200",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://picsum.photos/id/232/200/200",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://picsum.photos/id/231/200/200",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://picsum.photos/id/247/200/200",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://picsum.photos/id/235/200/200",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
        }
    }
}
</script>

<template>
    <section class="container">

        <div class="container-comics-list">
            <h2 class="title-section">CURRENT SERIES</h2>
            <div class="comics-list">
                <comicsBox class="comic-box" v-for="(element, index) in comicsList" :img="comicsList[index].thumb"
                    :series="comicsList[index].series" />
            </div>
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
            display: flex;
            flex-wrap: wrap;

            .comic-box {
                padding: 50px 10px;
                width: 190px;

                :deep(.comic) {
                    width: 190px;
                    padding-bottom: 10px;

                    img {
                        width: 100%;
                        margin: 0 auto;
                    }
                    .title {
                        text-transform: uppercase;
                    }
                }
            }
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