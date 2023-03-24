<script>
export default {
    data() {
        return {

            images: [
                '/img/footer-facebook.png',
                '/img/footer-periscope.png',
                '/img/footer-pinterest.png',
                '/img/footer-twitter.png',
                '/img/footer-youtube.png',

            ]

        }
    },

}
</script>

<template>
    <div class="container">

        <div class="inner-container">
            <div class="btn">
                <button>SIGN-UP NOW</button>
            </div>

            <div class="social">
                <div class="follow">FOLLOW US</div>
                <div class="links">
                    <img v-for="(image, index) in images" :src="image" alt="">

                </div>
            </div>

        </div>

    </div>
</template>

<style lang="scss" scoped>
.container {
    width: 100%;
    height: 80px;
    background-color: #303030;

    .inner-container {
        width: 1000px;
        height: 100%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .btn {
            button {
                background-color: #303030;
                padding: 12px;
                border: 2px solid #14538f;
                color: white;
                font-weight: bold;
            }
        }

        .social {
            display: flex;
            gap: 10px;

            .follow {
                color: #14538f;
                font-weight: bold;
                display: flex;
                align-items: center;
            }

            .links {
                display: flex;
                gap: 5px;
            }
        }
    }
}
</style>