<template>
    <div>
        <div class="row mb-5">
            <div class="col-3">
                <div v-text="label13"></div>
                <button type="button" class="btn btn-secondary mt-1">Default</button>
            </div>
            <div class="col-3">
                <div v-text="label14"></div>
                <button type="button" class="btn btn-primary mt-1">Default</button>
            </div>
            <div class="col-3">
                <div v-text="label15"></div>
                <button type="button" class="btn btn-secondary mt-1">Secondary</button>
            </div>
            <div class="col">
                <div v-text="label16"></div>
                <button type="button" class="btn btn-danger mt-1">Danger</button>
            </div>
        </div>

        <div class="row mb-5">
            <div v-text="label2"></div>
            <div class="col-3">
                <button type="button" class="btn btn-secondary mt-1">Default</button>
            </div>
            <div class="col-3">
                <button type="button" class="btn btn-primary mt-1">Default</button>
            </div>
            <div class="col-3">
                <button type="button" class="btn btn-secondary mt-1">Secondary</button>
            </div>
            <div class="col">
                <button type="button" class="btn btn-danger mt-1">Danger</button>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-color',
        data() {
            return {
                label2: '&:hover, &:focus',
                label13: '<Button color=”default” />',
                label14: '<Button color=”primary” />',
                label15: '<Button color=”secondary” />',
                label16: '<Button color=”danger” />'
            }
        }
    }
</script>

<style scoped>

</style>