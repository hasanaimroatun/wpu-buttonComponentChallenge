<template>
    <div class="row mb-5">
        <div class="col-md-4 col-sm-8">
            <div v-text="label6" class="label"></div>
            <button type="button" class="btnDisabled mt-1" @click="$emit('btnStyle5')">Disabled</button>
        </div>
        <div class="col-md-4 col-sm-8">
            <div v-text="label7" class="label lDisabledText"></div>
            <button type="button" class="btnDisabledText mt-1" @click="$emit('btnStyle6')">Disabled</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-disabled',
        data() {
            return {
                label6: '<Button disabled />',
                label7: '<Button variant=”text” disabled />'
            }
        },
        emits: ['btnStyle5', 'btnStyle6']
    }
</script>

<style scoped>
.lDisabledText {
    color: #333333;
}

button {
    padding: 7px 15px;
    border-radius: 6px;
}

.btnDisabled,
.btnDisabled:hover,
.btnDisabled:focus {
    background-color: #E0E0E0;
    border: none;
    color: #9E9E9E;
    outline: none;
}

.btnDisabledText,
.btnDisabledText:hover,
.btnDisabledText:focus {
    background-color: white;
    color: #9E9E9E;
    border: none;
    outline: none;
}

@media screen and (max-width:768px) {
    .lDisabledText {
        margin-top: 45px;
    }

    button {
        margin-left: 45px;
    }
}
</style>