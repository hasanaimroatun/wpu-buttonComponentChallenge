<template>
    <div class="row mb-5">
        <div class="col-md-9 col-sm-8">
            <div v-text="label4" class="label"></div>
            <button type="button" class="btn mt-1">Default</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-text',
        data() {
            return {
                label4: '<Button variant=”text” />'
            }
        }
    }
</script>

<style scoped>
.label {
    color: #333333;
}

button,
button:hover,
button:focus  {
    color: #3D5AFE;
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