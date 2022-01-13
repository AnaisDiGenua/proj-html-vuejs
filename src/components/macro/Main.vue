<template>
    <main>
        <Hero/>
        <Services/>
        <Videos/>
    </main>
</template>

<script>
import Hero from '../sections/Hero.vue';
import Services from '../sections/Services.vue';
import Videos from '../sections/Videos.vue';

export default {
    name: 'Main',
    components:  {
        Hero,
        Services,
        Videos
    }
}
</script>

<style>

</style>