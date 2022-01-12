<template>
    <header>
        <div class="container">
            <Logo/>
            <NavBar :links="navLinks"/>
        </div>
    </header>
</template>

<script>
import NavBar from '../commons/NavBar.vue';
import Logo from '../commons/Logo.vue';

export default {
    name: 'Header',
    components: {
        NavBar,
        Logo
    },
    data() {
        return {
            navLinks: [
                {
                    title: 'Home',
                    href: '#'
                },
                {
                    title: 'Services',
                    href: '#'
                },
                {
                    title: 'About',
                    href: '#'
                },
                {
                    title: 'Videos',
                    href: '#'
                },
                {
                    title: 'Blog',
                    href: '#'
                },
                {
                    title: 'Store',
                    href: '#'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    header {
        width: 100%;
        height: 100px;
        background-color: $darkColor;
        .container {
            height: 100%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
    }
</style>