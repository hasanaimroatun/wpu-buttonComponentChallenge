<template>
    <div class="row mb-5">
        <div class="col-4">
            <div v-text="label4"></div>
            <button type="button" class="btn btn-light mt-1">Default</button>
        </div>
        <div class="col">
            <div v-text="label2"></div>
            <button type="button" class="btn btn-light mt-1">Default</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-text',
        data() {
            return {
                label2: '&:hover, &:focus',
                label4: '<Button variant=”text” />'
            }
        }
    }
</script>

<style scoped>

</style>