<template>
    <div>
        <div class="row mb-5">
            <div class="col-md-3 col-sm-8">
                <div v-text="label13" class="label"></div>
                <button type="button" class="btn btnDefault mt-1">Default</button>
            </div>
            <div class="col-md-3 col-sm-8">
                <div v-text="label14" class="label lPrimary"></div>
                <button type="button" class="btn btnPrimary mt-1">Default</button>
            </div>
            <div class="col-md-3 col-sm-8">
                <div v-text="label15" class="label lSecondary"></div>
                <button type="button" class="btn btnSecondary mt-1">Secondary</button>
            </div>
            <div class="col-md-3 col-sm-8">
                <div v-text="label16" class="label lDanger"></div>
                <button type="button" class="btn btnDanger mt-1">Danger</button>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-color',
        data() {
            return {
                label13: '<Button color=”default” />',
                label14: '<Button color=”primary” />',
                label15: '<Button color=”secondary” />',
                label16: '<Button color=”danger” />'
            }
        }
    }
</script>

<style scoped>
.btnDefault {
    background-color: #E0E0E0;
    border: 1px solid #E0E0E0;
    color: #3F3F3F;
}

.btnDefault:hover,
.btnDefault:focus {
    background-color: #AEAEAE;
    border: 1px solid #AEAEAE;
}

.btnPrimary {
    background-color: #2962FF;
    border: 1px solid #2962FF;
    color: white;
}

.btnPrimary:hover,
.btnPrimary:focus {
    background-color: #0039CB;
    border: 1px solid #0039CB;
    color: white;
}

.btnSecondary {
    background-color: #455A64;
    border: 1px solid #455A64;
    color: white;
}

.btnSecondary:hover,
.btnSecondary:focus {
    background-color: #1C313A;
    border: 1px solid #1C313A;
    color: white;
}

.btnDanger {
    background-color: #D32F2F;
    border: 1px solid #D32F2F;
    color: white;
}

.btnDanger:hover,
.btnDanger:focus {
    background-color: #9A0007;
    border: 1px solid #9A0007;
    color: white;
}

@media screen and (max-width:768px) {
    .lPrimary,
    .lSecondary,
    .lDanger {
        margin-top: 45px;
    }

    button {
        margin-left: 45px;
    }
}

</style>