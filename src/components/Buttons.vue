<template>
    <div class="row g-0">
        <div class="col-2 offset-1 text-start">
            <Navigation />
        </div>
        <div class="col-9 text-start">
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
            <div class="mt-5">Icons: <a href="https://material.io/resources/icons/?style=round">https://material.io/resources/icons/?style=round</a></div>
            <div class="mt-5 mb-5">created by <a href="#">hasanaimroatun</a> - devChallenges.io</div>
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

<style scoped>

</style>