<template>
    <div class="row mb-5">
        <div class="col-4">
            <div v-text="label8"></div>
            <button type="button" class="btn btn-primary mt-1">
                <font-awesome-icon icon="fa-solid fa-cart-plus" />
                Default
            </button>
        </div>
        <div class="col">
            <div v-text="label9"></div>
            <button type="button" class="btn btn-primary mt-1">
                <font-awesome-icon icon="fa-solid fa-cart-plus" />
                Default
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

</style>