<template>
    <section>
        <div class="container">
            <!-- inizio colonna sinistra -->
            <div class="col sx">
                <img src="../../assets/img/logo.png" alt="photo logo">
                <p class="gray-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet et cumque, qui ullam enim aliquam esse debitis ipsam, dolor voluptates, eligendi consequatur error omnis quis iste similique.</p>
                <ul class="social-links">
                    <li><a href="#"><i class="fab fa-facebook-f"></i></a></li>
                    <li><a href="#"><i class="fab fa-twitter"></i></a></li>
                    <li><a href="#"><i class="fab fa-youtube"></i></a></li>
                    <li><a href="#"><i class="fab fa-instagram"></i></a></li>
                    <li><a href="#"><i class="fab fa-linkedin-in"></i></a></li>
                </ul>
            </div>
            <!-- /colonna sinistra -->

            <!-- inizio colonna centrale -->
            <div class="col md">
                <h4>Recent posts</h4>
                <ul>
                    <li v-for="(link,index) in links" :key="index"><a href="#">{{link}}</a></li>
                </ul>
            </div>
            <!-- /colonna centrale -->

            <!-- inizio colonna destra -->
            <div class="col dx">
                <h4>Contact information</h4>
                <div class="gray-text">4746 Tipple Road Michigan 48449</div>
                <p>Mobile: 1.800.000.0000</p>
                <p>Email: info@your-company.com</p>
            </div>
            <!-- /colonna destra -->

        </div>
    </section>
</template>

<script>
export default {
    name : 'FooterTop',
    props: {
        links: Array
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    .container {
        display: flex;
        .col {
            width: calc(100% /3 - 40px);
            text-align: center;
            margin: 20px;
            h4 {
                font-size: 1.125rem;
                text-transform: uppercase;
                margin-bottom: 30px;
            }
        }
        .col.sx {
            img {
                margin-bottom: 30px;
            }
            .gray-text {
                line-height: 1.6;
            }
            .social-links {
                display: flex;
                justify-content: center;
                margin-top: 35px;
                li {
                    margin: 10px;
                    i {
                        color: $hoverBtn1;
                    }
                }
            }
        }
        .col.md {
            li {
                margin-bottom: 20px;
                a {
                    color: $white;
                    &::before {
                        content: "\f054";
                        font-family: "Font Awesome 5 Free";
                        font-weight: 900;
                        display: inline-block;
                        font-size: .75rem;
                    }
                }
            }
        }
        .col.dx {
            .gray-text {
                margin-bottom: 10px;
            }
            p {
                font-weight: 700;
            }
        }
        
    }
</style>