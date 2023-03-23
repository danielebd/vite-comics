<script>
export default {
    name: 'FooterShop'
}
</script>

<template>
    <div id="big-container">
        <div class="container">
            <div class="part">
                <div class="img">
                    <img src="../assets/buy-comics-digital-comics.png" alt="">
                </div>
                <div class="img-word">DIGITAL COMICS</div>
            </div>
            <div class="part">
                <div class="img">
                    <img src="../assets/buy-comics-merchandise.png" alt="">
                </div>
                <div class="img-word">DC MERCHANDISE</div>
            </div>
            <div class="part">
                <div class="img">
                    <img src="../assets/buy-comics-subscriptions.png" alt="">
                </div>
                <div class="img-word">SUBSCRIPTION</div>
            </div>
            <div class="part">
                <div class="img">
                    <img src="../assets/buy-comics-shop-locator.png" alt="">
                </div>
                <div class="img-word">COMIC SHOP LOCATOR</div>
            </div>
            <div class="part">
                <div class="img">
                    <img src="../assets/buy-dc-power-visa.svg" alt="">
                </div>
                <div class="img-word">DC POWER VISA</div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;

#big-container {
    background-color: $secondaryColorBlue;

    .container {
        box-sizing: border-box;
        display: flex;
        justify-content: space-between;
        max-width: $bigContainer;
        margin: 0 auto;
        padding: 50px;

        .part {
            display: flex;
            align-items: center;
            color: white;

            .img {
                padding-right: 10px;

                img {
                    width: 55px;
                    height: 55px;
                    object-fit: contain;
                }
            }
        }
    }
}
</style>

