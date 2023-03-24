<script>
export default {
    data() {
        return {

            links: [
                'CHARACTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FANS',
                'NEWS',
                'SHOP'
            ]

        }
    },
}
</script>

<template>
    <div class="container">

        <header>
            <div class="img">
                <img src="/img/dc-logo.png" alt="">
            </div>

            <div class="links">
                <ul>
                    <li v-for="(link, index) in links"> {{ link }} </li>

                </ul>
            </div>
        </header>

    </div>
</template>

<style lang="scss" scoped>
@mixin container() {
    width: 1000px;
}

.container {
    @include container()
}

header {
    display: flex;
    justify-content: space-between;

    margin-top: 20px;

    .img {
        img {

            width: 60%;
        }
    }

    .links {
        ul {
            display: flex;
            gap: 12px;
            align-items: center;
            height: 100%;

            li {

                font-size: 11px;
                cursor: pointer;
                padding-bottom: 20px;
                position: relative;
                height: 100%;
                display: flex;
                align-items: center;

                &::after {
                    content: '';
                    height: 3px;
                    width: 100%;
                    background-color: #0283fa;
                    position: absolute;
                    bottom: 0;
                    left: 0;
                    display: none;
                }

                &:hover {

                    &::after {
                        display: inline-block;
                    }

                }


            }

        }
    }
}
</style>