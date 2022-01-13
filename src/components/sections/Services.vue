<template>
    <section>
        <div class="container">
            <CardServices/>
            <div class="quote-box">
                <div class="quote-content">
                    <p>"Lorem ipsum dolor sit amet consectetur adipisicing elit. Aperiam totam eos accusamus debitis adipisci ratione quisquam ipsa minima voluptatem rem, optio ut neque id explicabo assumenda, vitae earum omnis facere."</p>
                    <div class="author-box">
                        <img src="../../assets/img/avatar-1-2x.jpg" alt="avatar photo">
                        <span>Brad Johnson</span>
                        <span>Las Vegas</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import CardServices from '../commons/CardServices.vue';

export default {
    name: 'Services',
    components: {
        CardServices
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    section {
        height: 800px;
        background-image: linear-gradient(150deg, #4154ff 0%, #d5000b 100%);
        .author-box  {
            height: 44px;
            line-height: 44px;
            margin-top: 20px;
            span {
                color: rgba(255, 255, 255, 0.5);
            }
            span:first-of-type{
                font-weight: 700;
                color: $white;
                margin: 0 10px;
            } 
            img {
                width: 40px;
                border-radius: 50%;
                vertical-align: middle;
            } 
        }
    }

</style>