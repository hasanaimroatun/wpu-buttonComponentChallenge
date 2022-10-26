<template>
    <div class="row mb-5">
        <div class="col-4">
            <div v-text="label3"></div>
            <button type="button" class="btn btn-outline-primary mt-1">Default</button>
        </div>
        <div class="col">
            <div v-text="label2"></div>
            <button type="button" class="btn btn-outline-primary mt-1">Default</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-outline',
        data() {
            return {
                label2: '&:hover, &:focus',
                label3: '<Button variant=”outline” />'
            }
        }
    }
</script>

<style scoped>

</style>