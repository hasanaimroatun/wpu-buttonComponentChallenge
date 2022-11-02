<template>
    <div class="row mb-5">
        <div class="col-md-9 col-sm-8">
            <div v-text="label5" class="label"></div>
            <button type="button" class="btn mt-1" @click="$emit('btnStyle4')">Default</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-disableShadow',
        data() {
            return {
                label5: '<Button disableShadow />'
            }
        },
        emits: ['btnStyle4']
    }
</script>

<style scoped>
.label {
    color: #333333;
}

button,
button:hover,
button:focus {
    background-color: #3D5AFE;
    color: white;
    box-shadow: none;
}

@media screen and (max-width:768px) {
    button {
        margin-left: 45px;
    }
}
</style>