<template>
    <main>
        <Hero/>
        <Services/>
        <Videos/>
        <Subscription/>
        <Services2/>
        <Articles/>
    </main>
</template>

<script>
import Hero from '../sections/Hero.vue';
import Services from '../sections/Services.vue';
import Videos from '../sections/Videos.vue';
import Subscription from '../sections/Subscription.vue';
import Services2 from '../sections/Services2.vue';
import Articles from '../sections/Articles.vue';

export default {
    name: 'Main',
    components:  {
        Hero,
        Services,
        Videos,
        Subscription,
        Services2,
        Articles
    }
}
</script>

<style>

</style>