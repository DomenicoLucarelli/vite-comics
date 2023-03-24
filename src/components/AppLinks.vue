<script>
export default {
    data() {
        return {

            linksList: [
                {
                    title: 'DC COMICS',
                    links: [
                        'Characters',
                        'Comics',
                        'Movie',
                        'TV',
                        'Games',
                        'Video',
                        'News',
                    ],
                },

                {
                    title: 'DC COMICS',
                    links: [

                        'Terms of use',
                        'Privacy policy',
                        'Ad choices',
                        'Advertising',
                        'jobs',
                        'Subscriptions',
                        'Talent workshops',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop help',
                        'Contact Us',

                    ],
                },

                {
                    title: 'DC COMICS',
                    links: [
                        'DC',
                        'MAD Magazine',
                        'DC kids',
                        'DC Universe',
                        'DC Power Visa',

                    ],
                },


                {
                    title: 'DC COMICS',
                    links: [
                        'Shop DC',
                        'Shop DC Collectibles',

                    ],
                },



            ],

        }
    },
}
</script>

<template>
    <div class="container">

        <div class="inner-container">

            <div class="list-container">

                <div class="list-item" v-for="(item, index) in linksList">
                    <strong>{{ item.title }}</strong>
                    <ul>
                        <li v-for="(link, index) in linksList[index].links">{{ link }}</li>

                    </ul>
                </div>


            </div>

            <div class="image">
                <img src="/img/dc-logo-bg.png" alt="">
            </div>

        </div>

    </div>
</template>

<style lang="scss" scoped>
.container {
    width: 100%;
    height: 300px;
    background-image: url('/img/footer-bg.jpg');
    color: white;

    .inner-container {
        width: 1000px;
        height: 100%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;

        .list-container {



            display: flex;
            gap: 40px;
            padding: 10px 0;
            position: relative;
            max-width: 400px;
            width: 400px;

            .list-item {
                width: calc(100% / 3 - 40px);

                &:last-child {
                    position: absolute;
                    bottom: 30px;
                }

                ul {
                    li {
                        color: #726e66;
                        font-size: 12px;
                        font-weight: bold;
                    }
                }
            }
        }

        .image {
            height: 100%;
            overflow: hidden;

            img {
                height: 130%;
                position: relative;
                top: -45px;
            }
        }
    }
}
</style>