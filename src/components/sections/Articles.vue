<template>
    <section>
        <div class="container">
            <div class="title-box">
                <h5>Latest Articles</h5>
                <p>Read all articles <i class="fas fa-chevron-right"></i></p>
            </div>
            <CardArticle/>
        </div>
    </section>
</template>

<script>
import CardArticle from '../commons/CardArticle.vue';

export default {
    name: 'Articles',
    components: {
        CardArticle
    }
}
</script>

<style lang="scss" scoped>
</style>