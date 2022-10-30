<template>
    <div class="row g-0">
        <div class="col-2 offset-1 text-start">
            <Navigation />
        </div>
        <div class="col-8 text-start">
            <h1 class="mt-3">Buttons</h1>
            <ButtonDefault />
            <ButtonOutline />
            <ButtonText />
            <ButtonDisableShadow />
            <ButtonDisabled />
            <ButtonIcon />
            <ButtonSize />
            <ButtonColor />

            <br><br>
            <div class="iconSource mt-5">Icons: <a href="https://fontawesome.com/icons/cart-plus?s=solid&f=classic">https://fontawesome.com/icons/cart-plus?s=solid&f=classic</a></div>
            <div class="createdBy mt-5 mb-5">created by <a href="#">hasanaimroatun</a> - devChallenges.io</div>
        </div>
    </div>
</template>

<script>
    import ButtonDefault from './ButtonDefault.vue'
    import ButtonOutline from './ButtonOutline.vue'
    import ButtonText from './ButtonText.vue'
    import ButtonDisableShadow from './ButtonDisableShadow.vue'
    import ButtonDisabled from './ButtonDisabled.vue'
    import ButtonIcon from './ButtonIcon.vue'
    import ButtonSize from './ButtonSize.vue'
    import ButtonColor from './ButtonColor.vue'
    import Navigation from './Navigation.vue'

    export default {
        name: 'Button-component',
        components: {
            Navigation,
            ButtonDefault,
            ButtonOutline,
            ButtonText,
            ButtonDisableShadow,
            ButtonDisabled,
            ButtonIcon,
            ButtonSize,
            ButtonColor
        },
        data() {
            return {
                
            };
        }
    }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500;700&family=Noto+Sans:wght@500;700&family=Poppins:wght@500;600&family=Ubuntu+Mono&display=swap');

h1 {
    font-family: 'Poppins', sans-serif;
    font-weight: 500;
    font-size: 24px;
    line-height: 36px;
    color: #4F4F4F;
}

.label {
    font-family: 'Ubuntu Mono', monospace;
    font-weight: 400;
    font-size: 12px;
    line-height: 12px;
    color: #000000;
    margin-bottom: 12px;
}

button {
    font-family: 'Noto Sans', sans-serif;
    font-weight: 500;
}

.iconSource {
    font-family:  'Ubuntu Mono', monospace;
    font-weight: 400;
    font-size: 12px;
    line-height: 12px;
    color: #828282;
}

.createdBy {
    font-family: 'Montserrat', sans-serif;
    font-weight: 500;
    font-size: 14px;
    line-height: 17.07px;
    color: #A9A9A9;
}

.iconSource a,
.createdBy a {
    color: inherit;
    text-decoration: none;
}

.createdBy a {
    font-weight: 700;
}

.iconSource a:hover,
.createdBy a:hover {
    color: #4F4F4F;
}

@media screen and (max-width:768px) {
    h1,
    .label,
    .iconSource,
    .createdBy {
        padding-left: 45px;
    }
}
</style>