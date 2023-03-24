<script>
export default {
    data() {
        return {

            comics: [
                {
                    title: 'DIGITAL COMICS',
                    img: '/img/buy-comics-digital-comics.png',
                },

                {
                    title: 'DC MERCHANDISE',
                    img: '/img/buy-comics-merchandise.png',
                },

                {
                    title: 'SUBSCRIPTION',
                    img: '/img/buy-comics-shop-locator.png',
                },

                {
                    title: 'COMIC SHOP LOCATOR',
                    img: '/img/buy-comics-subscriptions.png',
                },

                {
                    title: 'DC POWER VISA',
                    img: '/img/buy-dc-power-visa.svg',
                }
            ],

        }
    },
}
</script>

<template>
    <div class="container">

        <div class="inner-container">

            <div class="item" v-for="(comic, index) in comics">
                <div class="image">
                    <img :src="comic.img" alt="">
                </div>

                <div class="text">
                    {{ comic.title }}
                </div>
            </div>

        </div>

    </div>
</template>

<style lang="scss" scoped>
.container {
    height: 120px;
    background-color: #0283fa;
    width: 100%;

    .inner-container {
        width: 1000px;
        margin: 0 auto;
        height: 100%;
        display: flex;

        .item {
            height: 100%;
            width: calc(100%/5);
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            font-size: 12px;
            color: white;

            .image {
                height: 100%;
                display: flex;
                align-items: center;
                justify-content: center;


                img {
                    height: 30%;
                }
            }
        }
    }

}
</style>