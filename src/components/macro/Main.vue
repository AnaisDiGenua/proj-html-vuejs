<template>
    <main>
        <Hero/>
        <Services/>
        <Videos/>
        <Subscription/>
    </main>
</template>

<script>
import Hero from '../sections/Hero.vue';
import Services from '../sections/Services.vue';
import Videos from '../sections/Videos.vue';
import Subscription from '../sections/Subscription.vue';

export default {
    name: 'Main',
    components:  {
        Hero,
        Services,
        Videos,
        Subscription
    }
}
</script>

<style>

</style>