<template>
    <div class="card-container">
        <div class="card">
            <img src="../../assets/img/blog4-2x-400x258.jpg" alt="article photo">
            <h5>The best protein shake</h5>
            <p class="gray-text">By Admin | November 26th, 2019 | Gym</p>
        </div>
        <div class="card">
            <img src="../../assets/img/blog1-2x-400x258.jpg" alt="article photo">
            <h5>Ultimate cardio workout</h5>
            <p class="gray-text">By Admin | November 26th, 2019 | Gym</p>
        </div>
        <div class="card">
            <img src="../../assets/img/blog3-2x-400x258.jpg" alt="article photo">
            <h5>New juices  available now</h5>
            <p class="gray-text">By Admin | November 26th, 2019 | Gym</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardArticle'
}
</script>

<style lang="scss" scoped>
    .card-container {
        display: flex;
        justify-content: center;
        .card {
            width: calc(100% / 3 - 40px); 
            margin: 20px;
            position: relative;
            img {
                width: 100%;
                margin-bottom: 20px;
            }
            .gray-text {
                font-size: .875rem;
                margin-top: 5px;
            }
        }
    }
</style>