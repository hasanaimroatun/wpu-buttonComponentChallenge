<template>
    <div class="row mt-2 mb-5">
        <div class="col-4">
            <div v-text="label1"></div>
            <button type="button" class="btn btn-secondary mt-1">Default</button>
        </div>
        <div class="col">
            <div v-text="label2"></div>
            <button type="button" class="btn btn-secondary mt-1">Default</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-default',
        data() {
            return {
                label1: '<Button />',
                label2: '&:hover, &:focus'
            }
        }
    }
</script>

<style scoped>

</style>