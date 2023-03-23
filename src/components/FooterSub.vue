<script>
export default {
    name: 'FooterSub'
}
</script>

<template>
    <div id="container">
        <div id="sub">
            <h3>SIGN-UP NOW!</h3>
            <div id="social">
                <h3>FOLLOW US</h3>
                <div class="box-icon"><i class="fa-brands fa-facebook-f"></i></div>
                <div class="box-icon"><i class="fa-brands fa-twitter"></i></div>
                <div class="box-icon"><i class="fa-brands fa-youtube"></i></div>
                <div class="box-icon"><i class="fa-brands fa-pinterest-p"></i></div>
                <div class="box-icon"><i class="fa-solid fa-location-dot"></i></div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss' as *;

#container {
    background-color: #303030;

    #sub {
        max-width: $bigContainer;
        margin: 0 auto;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 30px 0;

        &>h3 {
            color: white;
            padding: 13px;
            margin: 0;
            border: solid $primaryColorBlue 2px;
            &:hover {
                        cursor: pointer;
                    }
        }

        #social {
            h3 {
                display: inline-block;
                color: $primaryColorBlue;
            }

            div {
                display: inline-block;
                width: 35px;
                background-color: #797979;
                text-align: center;
                line-height: 35px;
                border-radius: 50px;
                vertical-align: middle;
                margin-left: 20px;
                &:hover {
                        cursor: pointer;
                    }

                i {
                    font-size: 22px;
                    vertical-align: middle;
                    color: #303030;

                    
                }
            }
        }
    }
}
</style>