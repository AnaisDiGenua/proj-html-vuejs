<template>
    <div class="card-container">
        <div class="card">
            <i class="fas fa-clock"></i>
            <h4>Team training</h4>
            <p class="yellow-text">Find a partner</p>
            <p class="text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores asperiores ullam, voluptatem recusandae qui quae ut voluptates.</p>
            <p>Find a partner<i class="fas fa-chevron-right"></i></p>
        </div>
        <div class="card">
            <i class="fas fa-dumbbell"></i>
            <h4>Crossfit workout</h4>
            <p class="yellow-text">Push your limits</p>
            <p class="text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores asperiores ullam, voluptatem recusandae qui quae ut voluptates.</p>
            <p>Learn about crossfit<i class="fas fa-chevron-right"></i></p>
        </div>
        <div class="card">
            <i class="fas fa-fire-alt"></i>
            <h4>Weight loss plan</h4>
            <p class="yellow-text">Shed those pound</p>
            <p class="text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores asperiores ullam, voluptatem recusandae qui quae ut voluptates.</p>
            <p>Schedule a workout<i class="fas fa-chevron-right"></i></p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardService2'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    .card-container {
        display: flex;
        justify-content: center;
        .card {
            width: calc(100% / 3 - 40px);
            margin: 40px;
            text-align: center;
            padding: 40px 30px;
            border: 2px solid $btn1;
            p:last-child {
                color: $white;
                margin-top: 20px
            }
            i.fa-chevron-right {
                font-size: .625rem;
                margin-left: 4px;
            }
            .text {
                line-height: 1.4;
                color: rgba(255, 255, 255, 0.4);
            }
            i{
                font-size: 2.1875rem;
                color: $white;
                margin-bottom: 15px;
            }
            .yellow-text {
                margin: 5px 0 30px;
            }
        }
    }
</style>