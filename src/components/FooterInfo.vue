<script>
export default {
    name: 'FooterInfo'
}
</script>

<template>
    <div class="big-container">
        <div class="container">
            <div id="container-columns">
                <div id="column">
                    <div id="part-1">
                        <h1>DC COMICS</h1>
                        <ul class="content">
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                    </div>
                    <div id="part-2">
                        <h1>SHOP</h1>
                        <ul class="content">
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </div>
                </div>
                <div id="column">
                    <h1>DC</h1>
                    <ul class="content">
                        <li>Term Of Use</li>
                        <li>Privacy policy(NEW)</li>
                        <li>Ad Choises</li>
                        <li>Advertaising</li>
                        <li>Jobs</li>
                        <li>Subscriptioning</li>
                        <li>Talent Workshop</li>
                        <li>CPSC Certificates</li>
                        <li>Rating</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div id="column">
                    <h1>SITES</h1>
                    <ul class="content">
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa </li>
                    </ul>
                </div>
            </div>

            <div class="img">
                <img src="../assets/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;

.big-container {
    background-image: url("../assets/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    color: white;

    .container {
        max-width: $bigContainer;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;

        #container-columns {
            display: flex;

            #column {
                margin-top: 30px;
                margin-right: 70px;

                h1 {
                    font-size: 21px;
                    margin: 0;
                }

                ul {
                    padding: 0;
                    list-style-type: none;

                    li {
                        line-height: 22px;
                        color: rgba(211, 211, 211, 0.384);
                        font-size: smaller;
                    }
                }
            }
        }

        .img {
            width: 570px;
            height: 370px;
        }

        img {
            width: 570px;
            height: 100%;
            object-fit: cover;
        }


    }
}
</style>