<template>
    <div class="row mb-5">
        <div class="col-md-9 col-sm-8">
            <div v-text="label3" class="label"></div>
            <button type="button" class="btn mt-1" @click="$emit('btnStyle2')">Default</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-outline',
        data() {
            return {
                label3: '<Button variant=”outline” />'
            }
        },
        emits: ['btnStyle2']
    }
</script>

<style scoped>
.label {
    color: #333333;
}

button,
button:hover,
button:focus {
    color: #3D5AFE;
    border: 1px solid #3D5AFE;
}

button:hover,
button:focus {
    background-color: #ccebff;
}

@media screen and (max-width:768px) {
    button {
        margin-left: 45px;
    }
}
</style>