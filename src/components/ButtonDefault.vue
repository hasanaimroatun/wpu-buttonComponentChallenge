<template>
    <div class="row mb-5">
        <div class="col-md-9 col-sm-8">
            <div v-text="label1" class="label"></div>
            <button type="button" class="btn mt-1">Default</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-default',
        data() {
            return {
                label1: '<Button />'
            }
        }
    }
</script>

<style scoped>
.label {
    color: #333333;
    margin-top: 28px;
}

button {
    background-color: #E0E0E0;
    border: 1px solid #E0E0E0;
    color: #3F3F3F;
}

button:hover,
button:focus {
    background-color: #AEAEAE;
    border: 1px solid #AEAEAE;
}

@media screen and (max-width:768px) {
    button {
        margin-left: 45px;
    }
}
</style>