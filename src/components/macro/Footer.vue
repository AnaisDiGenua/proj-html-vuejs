<template>
    <footer>
        <FooterTop :links="footerLinks"/>
        <hr>
        <FooterBottom/>
    </footer>
</template>

<script>
import FooterTop from '../sections/FooterTop.vue';
import FooterBottom from '../sections/FooterBottom.vue';

export default {
    name: 'Footer',
    components: {
        FooterTop,
        FooterBottom
    },
    data() {
        return {
            footerLinks: [
                'The best protein shake',
                'Ultimate cardio workout',
                'New juices available now',
                'Tips to find training partners',
                '20 best healthy recipes'
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    footer {
        background-color: $darkColor;
    }
    hr {
        color: $gray;
    }

</style>