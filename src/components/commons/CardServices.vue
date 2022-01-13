<template>
    <div class="card-container">
        <div class="card">
            <img src="../../assets/img/service6-2x.jpg" alt="crossfit workout photo">
            <div class="content-box">
                <h4>Crossfit workout</h4>
                <p class="yellow-text">Push your limits</p>
            </div>
        </div>
        <div class="card">
            <img src="../../assets/img/box1-2x.jpg" alt="gym apparel photo">
            <div class="content-box">
                <h4>New gym appareal</h4>
                <p class="yellow-text">Look good, feel good</p>
            </div>
        </div>
        <div class="card">
            <img src="../../assets/img/box3-2x.jpg" alt="team training photo">
            <div class="content-box">
                <h4>Team training</h4>
                <p class="yellow-text">Find a partner</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardServices'
}
</script>

<style lang="scss" scoped>
    .card-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            position: relative;
            bottom: 80px;
            .card {
                width: calc(90% / 3 - 40px); 
                height: 300px;
                margin: 20px;
                border-radius: 2px 2px 20px 2px;
                overflow: hidden;
                position: relative;
                cursor: pointer;
                img {
                    width: 300px;
                    object-fit: cover;
                }
                .content-box {
                    position: absolute;
                    bottom: 20px;
                    left: 20px;
                }
            }
        }
    
</style>