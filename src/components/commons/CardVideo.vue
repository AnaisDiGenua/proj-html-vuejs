<template>
    <div class="card-container">
        <div class="card">
            <img src="../../assets/img/video2-2x.jpg" alt="video photo">
            <h5>Thighs & glute workout</h5>
            <p class="blue-text">Increase your mobility</p>
            <div class="play-btn">
                <i class="fas fa-play"></i>
            </div>
        </div>
        <div class="card">
            <img src="../../assets/img/video7-2x.jpg" alt="video photo">
            <h5>Lift, firm & perk up</h5>
            <p class="blue-text">Feel young again</p>
            <div class="play-btn">
                <i class="fas fa-play"></i>
            </div>
        </div>
        <div class="card">
            <img src="../../assets/img/video9-2x.jpg" alt="video photo">
            <h5>Slim & trim ypour waist</h5>
            <p class="blue-text">Shed those extra punds</p>
            <div class="play-btn">
                <i class="fas fa-play"></i>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardVideo'
}
</script>

<style lang="scss" scoped>
    .card-container {
        display: flex;
        justify-content: center;
        .card {
            width: calc(100% / 3 - 40px); 
            margin: 20px;
            text-align: center;
            position: relative;
            img {
                width: 100%;
                border-radius: 2px 2px 20px 2px;
                margin-bottom: 20px;
            }
            .blue-text {
                font-size: .875rem;
                margin-top: 5px;
            }
            .play-btn {
                width: 40px;
                height: 40px;
                line-height: 40px;
                top: 30%;
                left: 45%;
                    i {
                        font-size: .5rem;
                        cursor: pointer;
                    }
                }
            }
    }
</style>