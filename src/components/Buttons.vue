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
            <div class="row mt-2 mb-5">
                <div class="col-4">
                    <div v-text="label1"></div>
                    <button type="button" class="btn btn-secondary mt-1">Default</button>
                </div>
                <div class="col">
                    <div v-text="label2"></div>
                    <button type="button" class="btn btn-secondary mt-1">Default</button>
                </div>
            </div>

            <div class="row mb-5">
                <div class="col-4">
                    <div v-text="label3"></div>
                    <button type="button" class="btn btn-outline-primary mt-1">Default</button>
                </div>
                <div class="col">
                    <div v-text="label2"></div>
                    <button type="button" class="btn btn-outline-primary mt-1">Default</button>
                </div>
            </div>

            <div class="row mb-5">
                <div class="col-4">
                    <div v-text="label4"></div>
                    <button type="button" class="btn btn-light mt-1">Default</button>
                </div>
                <div class="col">
                    <div v-text="label2"></div>
                    <button type="button" class="btn btn-light mt-1">Default</button>
                </div>
            </div>

            <div class="row mb-5">
                <div class="col-4">
                    <div v-text="label5"></div>
                    <button type="button" class="btn btn-primary mt-1">Default</button>
                </div>
                <div class="col">
                    <div v-text="label2"></div>
                    <button type="button" class="btn btn-primary mt-1">Default</button>
                </div>
            </div>

            <div class="row mb-5">
                <div class="col-4">
                    <div v-text="label6"></div>
                    <button type="button" class="btn btn-secondary mt-1" disabled data-bs-toggle="button">Disabled</button>
                </div>
                <div class="col">
                    <div v-text="label7"></div>
                    <button type="button" class="btn btn-light mt-1" disabled data-bs-toggle="button">Disabled</button>
                </div>
            </div>

            <div class="row mb-5">
                <div class="col-4">
                    <div v-text="label8"></div>
                    <button type="button" class="btn btn-primary mt-1">
                        <font-awesome-icon icon="fa-solid fa-cart-plus" />
                        Default
                    </button>
                </div>
                <div class="col">
                    <div v-text="label9"></div>
                    <button type="button" class="btn btn-primary mt-1">
                        <font-awesome-icon icon="fa-solid fa-cart-plus" />
                        Default
                    </button>
                </div>
            </div>

            <div class="row mb-5">
                <div class="col-3">
                    <div v-text="label10"></div>
                    <button type="button" class="btn btn-primary btn-sm mt-1">Default</button>
                </div>
                <div class="col-3">
                    <div v-text="label11"></div>
                    <button type="button" class="btn btn-primary btn-md mt-1">Default</button>
                </div>
                <div class="col">
                    <div v-text="label12"></div>
                    <button type="button" class="btn btn-primary btn-lg mt-1">Default</button>
                </div>
            </div>

            <div class="row mb-5">
                <div class="col-3">
                    <div v-text="label13"></div>
                    <button type="button" class="btn btn-secondary mt-1">Default</button>
                </div>
                <div class="col-3">
                    <div v-text="label14"></div>
                    <button type="button" class="btn btn-primary mt-1">Default</button>
                </div>
                <div class="col-3">
                    <div v-text="label15"></div>
                    <button type="button" class="btn btn-secondary mt-1">Secondary</button>
                </div>
                <div class="col">
                    <div v-text="label16"></div>
                    <button type="button" class="btn btn-danger mt-1">Danger</button>
                </div>
            </div>

            <div class="row mb-5">
                <div v-text="label2"></div>
                <div class="col-3">
                    <button type="button" class="btn btn-secondary mt-1">Default</button>
                </div>
                <div class="col-3">
                    <button type="button" class="btn btn-primary mt-1">Default</button>
                </div>
                <div class="col-3">
                    <button type="button" class="btn btn-secondary mt-1">Secondary</button>
                </div>
                <div class="col">
                    <button type="button" class="btn btn-danger mt-1">Danger</button>
                </div>
            </div>

            <br><br>
            <div class="mt-5">Icons: <a href="https://material.io/resources/icons/?style=round">https://material.io/resources/icons/?style=round</a></div>
            <div class="mt-5 mb-5">created by <a href="#">hasanaimroatun</a> - devChallenges.io</div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Button-component',
        data() {
            return {
                label1: '<Button />',
                label2: '&:hover, &:focus',
                label3: '<Button variant=”outline” />',
                label4: '<Button variant=”text” />',
                label5: '<Button disableShadow />',
                label6: '<Button disabled />',
                label7: '<Button variant=”text” disabled />',
                label8: '<Button startIcon=”local_grocery_store” />',
                label9: '<Button endIcon=”local_grocery_store” />',
                label10: '<Button size=”sm” />',
                label11: '<Button size=”md” />',
                label12: '<Button size=”lg” />',
                label13: '<Button color=”default” />',
                label14: '<Button color=”primary” />',
                label15: '<Button color=”secondary” />',
                label16: '<Button color=”danger” />'
            };
        }
    }
</script>

<style scoped>

</style>