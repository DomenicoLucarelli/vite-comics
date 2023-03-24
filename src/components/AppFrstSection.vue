<script>
export default {
    data() {
        return {

        }
    },
}
</script>

<template>
    <div class="container">

        <section>
            Contents goes here
        </section>

    </div>
</template>

<style lang="scss" scoped>
@mixin container() {
    width: 1000px;

}

.container {
    width: 100%;
    background-color: black;

}





section {
    @include container();

    height: 100px;

    color: white;

    display: flex;
    justify-content: center;
    align-items: center;
}
</style>