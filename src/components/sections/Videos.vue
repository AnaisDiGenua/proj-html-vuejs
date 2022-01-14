<template>
    <section>
        <!-- inizio youtube channel info -->
        <div class="yt-channel-box">
            <div class="photo-box">
                <img src="../../assets/img/service15-2x.jpg" alt="yt photo">
            </div>
            <div class="content-box">
                <p class="blue-text">Tune up your workouts</p>
                <h2>The best health & fitness <br> online</h2>
                <div class="channel">
                    <img src="../../assets/img/unnamed.jpg" alt="channel logo">
                    <div class="channel-info">
                        <p>ThemeFusion</p>
                        <button><i class="fab fa-youtube"></i>YouTube <span>999+</span></button>
                    </div>
                </div>
                <p class="gray-text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Modi, nam eaque! Alias, nihil nobis officia .</p>
                <button class="btn btn3"><i class="fab fa-youtube"></i>Visit my YouTube channel</button>
            </div>
        </div>
        <!-- /youtube channel info -->

        <!-- inizio playlist  -->
        <div class="container">
            <div class="title-box">
                <h5>Featured playlist</h5>
                <p>view all videos <i class="fas fa-chevron-right"></i></p>
            </div>
            <CardVideo/>
        </div>
        <!-- /playlist -->
    </section>
</template>

<script>
import CardVideo from '../commons/CardVideo.vue';

export default {
    name: 'Videos',
    components: {
        CardVideo
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    section {
        padding-top: 0;
    }
        .yt-channel-box {
            display: flex;
            > * {
                width: 50%;
            }
            .photo-box {
                height: 700px;
                overflow: hidden;
                border-radius: 2px 2px 20px 2px;
                img {
                    width: 100%;
                    object-fit: cover;
                }
            }
            .content-box {
                padding: 100px ;
                .channel {
                    display: flex;
                    margin: 10px 0 20px;
                    .channel-info {
                        margin-left: 10px;
                        p {
                            font-size: .75rem;
                            color: $gray;
                            margin-bottom: 3px;
                        }
                        button {
                            padding: 4px 0 4px 8px;
                            background-color:#e62117;
                            border: none;
                            color: $white;
                            i {
                                margin-right: 3px;
                            }
                            span {
                                background-color: #fafafa;
                                border: 1px solid lightgray;
                                padding: 4px 8px;
                                color: $gray;
                            }
                        }
                    }
                }
                .btn3 {
                    margin-top: 20px;
                    i {
                        margin-right: 4px;
                    }
                }
            }
        }
        .container {
            margin-top: 100px;
        }
        
</style>