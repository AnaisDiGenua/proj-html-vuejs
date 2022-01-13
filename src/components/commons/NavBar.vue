<template>
    <nav>
        <!-- inizio nav sinistra -->
        <ul class="nav-left">
            <li v-for="(link, index) in links" :key="index" @click="selectLink(index)">
                <a :href="link.href" :class="currentLink == index ? 'active' : '' " >{{link.title}}</a>
            </li>
        </ul>
        <!-- /nav sinistra -->

        <!-- inizio nav destra -->
        <ul class="nav-right">
            <li><button class="btn btn1">Schedule a workout</button></li>
            <li><i class="fas fa-search"></i></li>
            <li><i class="fas fa-shopping-cart"></i></li>
        </ul>
        <!-- /nav destra -->
    </nav>
</template>

<script>
export default {
    name: 'NavBar',
    props: {
        links: Array
    },
    data() {
        return {
            currentLink: 0
        }
    },
    methods: {
        selectLink(index) {
            this.currentLink = index;
            console.log(index);
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

    nav {
        color: white;
        display: flex;
        li {
            display: inline-block;
            margin-right: 30px;
        }
    }

    .nav-left {
        margin-right: 20px;
        height: 36px;
        line-height: 36px;
        li {
            a {
            color: $gray;
            font-size: 1.125rem;
                &.active, &:hover {
                    color: $white;
                }
            }
            &:last-child::after {
            content: 'new';
            display: inline;
            font-size: .875rem;
            color: black;
            background-color: $yellow;
            border-radius: 2px;
            margin-left: 10px;
            padding: 2px 6px ;
            }
        }
    }

    .nav-right {
        i {
            color: $gray;
            cursor: pointer;
            &:hover {
                color: $white;
            }
        }
    }
</style>