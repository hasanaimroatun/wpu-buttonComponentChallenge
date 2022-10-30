<template>
    <div class="row mb-5">
        <div class="col-md-4 col-sm-8">
            <div v-text="label8" class="label"></div>
            <button type="button" class="btn btn-primary mt-1">
                <font-awesome-icon icon="fa-solid fa-cart-plus" />
                Default
            </button>
        </div>
        <div class="col-md-4 col-sm-8">
            <div v-text="label9" class="label labelRight"></div>
            <button type="button" class="btn btn-primary mt-1">
                Default
                <font-awesome-icon icon="fa-solid fa-cart-plus" />
            </button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-icon',
        data() {
            return {
                label8: '<Button startIcon=”local_grocery_store” />',
                label9: '<Button endIcon=”local_grocery_store” />'
            }
        }
    }
</script>

<style scoped>
button {
    background-color: #2962FF;
}

@media screen and (max-width:768px) {
    .labelRight {
        margin-top: 45px;
    }

    button {
        margin-left: 45px;
    }
}
</style>