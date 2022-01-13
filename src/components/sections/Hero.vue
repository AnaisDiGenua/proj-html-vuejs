<template>
    <section>
        <div class="container">
            <!-- inizio contenuto -->
            <div class="content">
                <p class="red-text">Certified fitness professional</p>
                <h1>Take control of your health</h1>
                <p class="gray-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                <button class="btn btn1"><i class="fab fa-youtube"></i>Visit my Youtube channel</button>
                <button class="btn btn2">Buy Avada today<i class="fas fa-arrow-right"></i></button>
            </div>
            <!-- /contenuto -->
            <!-- play button -->
            <div class="play-btn">
                <i class="fas fa-play"></i>
            </div>
            <!-- /play button -->
        </div>
        <!-- sale button -->
        <div class="sale-btn">
            <div class="box">
                <i class="fas fa-id-card-alt"></i> 
                <p>Demos</p>
            </div>
            <div class="box">
                <p class="green-text">39</p>
                <p>On sale</p>
            </div>
        </div>
        <!-- /sale button -->
    </section>
</template>

<script>
export default {
    name: 'Hero'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    section {
        height: 500px; 
        background-image: url(../../assets/img/slider82x-scaled.jpg);
        background-size: cover;
        background-position: top;
        color: white;
        position: relative;
        .content {
            position: absolute;
            top: 50%;
            transform: translateY( -70%);
            h1 {
            font-size: 3rem;
            margin: 10px 0 20px 0;
            }
            .gray-text {
                color: $gray;
            }
            button {
                margin: 20px 10px 20px 0;
                i {
                    margin: 0 5px;
                }
            }
        }
        .play-btn {
            width: 70px;
            height: 70px;
            line-height: 70px;
            text-align: center;
            background-color: white;
            border-radius: 50%;
            position: absolute;
            top: 45%;
            left: 75%;
            transform: translate(-50%, -50%);
            i {
                color: $btn1;
                font-size: .75rem;
            }
        }
        .sale-btn {
            position: absolute;
            top: 20%;
            left: 97%;
            transform: translate(-50%, -50%);
            .box {
                width: 55px;
                background-color: $white;
                text-align: center;
                color: rgb(82, 82, 82);
                border-radius: 5px;
                padding: 5px 8px;
                margin-bottom: 10px;
                i {
                    font-size: 1.25rem;
                    margin-bottom: 5px;
                }
                p {
                    font-size: .75rem;
                    &.green-text{
                        font-size: 1.375rem;
                        font-weight: 700;
                        color: rgb(114, 189, 114);
                        &::before {
                            content: '$';
                            display: inline-block;
                            font-size: .9375rem;
                            position: relative;
                            bottom: 5px;
                        }
                    }
                }
            }
        }
    }
</style>