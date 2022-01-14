<template>
    <div class="container">
        <p class="gray-text">&#169; Copyrigth 2012 - 2020 | Avada theme by <span>ThemeFusion</span> | All rights reserved | Powered by <span>Wordpress</span></p>
    </div>
</template>

<script>
export default {
    name: 'FooterBottom'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    .container {
        padding: 30px 0;
        text-align: center;
        p {
            font-size: .875rem;
            span {
                font-weight: 700;
                color: $white;

            }
        }
    }
</style>