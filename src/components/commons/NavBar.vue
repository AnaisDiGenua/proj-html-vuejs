<template>
    <nav>
        <ul class="nav-left">
            <li>sinistra</li>
        </ul>
        <ul class="nav-right">
            <li>destra</li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'NavBar'
}
</script>

<style lang="scss" scoped>
    nav {
        color: white;
        display: flex;
    }

    .nav-left {
        margin-right: 20px;
    }
</style>