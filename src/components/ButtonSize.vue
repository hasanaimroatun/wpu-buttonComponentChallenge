<template>
    <div class="row mb-5">
        <div class="col-md-3 col-sm-8">
            <div v-text="label10" class="label"></div>
            <button type="button" class="btn btn-primary btn-sm mt-1" @click="$emit('btnStyle9')">Default</button>
        </div>
        <div class="col-md-3 col-sm-8">
            <div v-text="label11" class="label labelMd"></div>
            <button type="button" class="btn btn-primary btn-md mt-1" @click="$emit('btnStyle10')">Default</button>
        </div>
        <div class="col-md-3 col-sm-8">
            <div v-text="label12" class="label labelLg"></div>
            <button type="button" class="btn btn-primary btn-lg mt-1" @click="$emit('btnStyle11')">Default</button>
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
        },
        emits: ['btnStyle9', 'btnStyle10', 'btnStyle11']
    }
</script>

<style scoped>
button {
    background-color: #2962FF;
}

@media screen and (max-width:768px) {
    .labelMd,
    .labelLg {
        margin-top: 45px;
    }

    button {
        margin-left: 45px;
    }
}
</style>