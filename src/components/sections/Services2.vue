<template>
    <section>
        <div class="container">
            <CardService2/>
        </div>
    </section>
</template>

<script>
import CardService2 from '../commons/CardService2';

export default {
    name: 'Services2',
    components: {
        CardService2
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    section {
        background-color: $darkColor;
    }
</style>