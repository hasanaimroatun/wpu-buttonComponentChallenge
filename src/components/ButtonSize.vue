<template>
    <div class="row mb-5">
        <div class="col-3">
            <div v-text="label10"></div>
            <button type="button" class="btn btn-primary btn-sm mt-1">Default</button>
        </div>
        <div class="col-3">
            <div v-text="label11"></div>
            <button type="button" class="btn btn-primary btn-md mt-1">Default</button>
        </div>
        <div class="col">
            <div v-text="label12"></div>
            <button type="button" class="btn btn-primary btn-lg mt-1">Default</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-size',
        data() {
            return {
                label10: '<Button size=”sm” />',
                label11: '<Button size=”md” />',
                label12: '<Button size=”lg” />'
            }
        }
    }
</script>

<style scoped>

</style>