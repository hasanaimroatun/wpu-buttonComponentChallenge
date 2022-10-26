<template>
    <div class="row g-0">
        <div class="col-2 offset-1 text-start">
            <div class="mb-5"><b><span>Dev</span>challenges.io</b></div>
            <div class="navBar">
                <ul class="navbar-nav pe-3">
                    <li class="nav-item mb-3">
                        <a class="nav-link" href="#">Colors</a>
                    </li>
                    <li class="nav-item mb-3">
                        <a class="nav-link" href="#">Typography</a>
                    </li>
                    <li class="nav-item mb-3">
                        <a class="nav-link" href="#">Spaces</a>
                    </li>
                    <li class="nav-item mb-3">
                        <a class="nav-link" href="#">Buttons</a>
                    </li>
                    <li class="nav-item mb-3">
                        <a class="nav-link" href="#"><b>Inputs</b></a>
                    </li>
                    <li class="nav-item mb-3">
                        <a class="nav-link" href="#">Grid</a>
                    </li>
                </ul>
            </div>
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

    export default {
        name: 'Button-component',
        components: {
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