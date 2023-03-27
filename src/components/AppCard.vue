<script>
export default {



    data() {
        return {

        }
    },

    props: {
        imageUrl: String,
        title: String,
    }
}
</script>

<template>
    <div class="card">
        <div id="img">
            <img :src="imageUrl" alt="">
        </div>

        <div id="title"> {{ title }} </div>

    </div>
</template>

<style lang="scss" scoped>
.card {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: calc(100% / 6 - 20px);

    #img {
        img {
            width: 150px;
            height: 150px;
            object-fit: cover;
        }
    }

    #title {

        font-weight: bold;
        text-transform: uppercase;
        color: white;
        font-size: 0.7em;
        color: #d4e1bb;
    }
}
</style>