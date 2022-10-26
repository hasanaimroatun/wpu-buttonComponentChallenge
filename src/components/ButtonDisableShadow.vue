<template>
    <div class="row mb-5">
        <div class="col-4">
            <div v-text="label5"></div>
            <button type="button" class="btn btn-primary mt-1">Default</button>
        </div>
        <div class="col">
            <div v-text="label2"></div>
            <button type="button" class="btn btn-primary mt-1">Default</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-disableShadow',
        data() {
            return {
                label2: '&:hover, &:focus',
                label5: '<Button disableShadow />'
            }
        }
    }
</script>

<style scoped>

</style>