<template>
    <div>
        <div class="title"><b><span>Dev</span>challenges.io</b></div>
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
</template>

<script>
    export default {
        name: 'Navigation-bar'
    }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500;700&family=Noto+Sans:wght@500;700&family=Poppins:wght@500;600&family=Ubuntu+Mono&display=swap');

.title {
    font-family: 'Poppins', sans-serif;
    font-weight: 600;
    font-size: 13px;
    line-height: 19.5px;
    color: #090F31;
    margin-bottom: 122px;
}

.title span {
    color: #F7542E;
}

.navBar {
    font-family: 'Noto Sans', sans-serif;
    font-weight: 500;
    font-size: 14px;
    line-height: 20.27px;
    color: #9E9E9E;
}

.nav-link b {
    color: #090F31;
}


</style>