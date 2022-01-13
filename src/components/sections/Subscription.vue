<template>
    <section>
        <div class="container">
            <div class="content">
                <p class="red-text">Join our mailing list today</p>
                <h2>Insider offers & flash sales in your inbox every week</h2>
                <form>
                    <input type="text" placeholder="Insert your email...*">
                    <button class="btn btn1">Subscribe</button>
                </form>
                <p class="gray-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Aperiam, et porro? Veritatis alias, inventore velit nobis aliquam voluptate voluptatibus magnam voluptas similique. </p>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Subscription'
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    section {
        height: 550px;
        background-image: url(../../assets/img/banner1-2x.jpg);
        background-size: cover;
        background-position: top;
        .container {
            position: relative;
            .content {
                width: 60%;
                position: absolute;
                top: 0;
                h2 {
                    color: $white;
                    margin: 10px 0 20px 0;
                }
                button {
                    margin: 20px 10px 20px 0;
                    i {
                        margin: 0 5px;
                    }
                }
                form {
                    input {
                    width: 50%;
                    border-radius: 20px;
                    border: none;
                    padding: 12px 25px;
                    margin-right: 20px;
                    }
                    button {
                        padding: 12px 70px;
                    }
                }
            }
        }
    }
</style>