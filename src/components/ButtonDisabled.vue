<template>
    <div class="row mb-5">
        <div class="col-4">
            <div v-text="label6"></div>
            <button type="button" class="btn btn-secondary mt-1" disabled data-bs-toggle="button">Disabled</button>
        </div>
        <div class="col">
            <div v-text="label7"></div>
            <button type="button" class="btn btn-light mt-1" disabled data-bs-toggle="button">Disabled</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-disabled',
        data() {
            return {
                label6: '<Button disabled />',
                label7: '<Button variant=”text” disabled />'
            }
        }
    }
</script>

<style scoped>

</style>