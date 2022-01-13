<template>
    <main>
        <Hero/>
        <Services/>
    </main>
</template>

<script>
import Hero from '../sections/Hero.vue';
import Services from '../sections/Services.vue';

export default {
    name: 'Main',
    components:  {
        Hero,
        Services
    }
}
</script>

<style>

</style>