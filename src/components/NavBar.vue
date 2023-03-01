<template>
    <div id="navbar">
        <div class="navbar navbar-primary">
        <div class="navbar-logo"><a href="#">Logo</a></div>
        <nav class="nav-menu">
            <ul class="nav-list">
            <li class="nav-item active"><a href="#" class="nav-link">Link 1</a>
            <span class="d-block decorated-line-link"></span>
            </li>
            <li class="nav-item"><a href="#" class="nav-link">Link 2</a>
                <span class="d-block decorated-line-link"></span>
            </li>
            <li class="nav-item"><a href="#" class="nav-link">Link 3</a>
                <span class="d-block decorated-line-link"></span>
            </li>
            <li class="nav-item"><a href="#" class="nav-link">Link 4</a>
                <span class="d-block decorated-line-link"></span>
            </li>
            </ul>
        </nav>
        <div class="toggler">
            <div class="toggler-icon">
                <span class="bar"></span>
                <span class="bar"></span>
                <span class="bar"></span>
            </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'NavBar'
    }
</script>

<style lang="scss">
    @import '@/assets/scss/global';
</style>