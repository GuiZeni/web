<script setup>
import Background from '@/components/Background.vue';
import HeaderTop from '@/components/HeaderTop.vue';
import Scope from '@/components/Scope.vue';
import HowWorks from '@/components/HowWorks.vue';
import Experience from './components/Experience.vue'
import Contat from './components/Contat.vue'
import Footer from './components/Footer.vue'

</script>

<template>
  <div class="container">
    <Background />

    <div class="scope-overlay" id="inicio">
      <Scope />
    </div>

    <HeaderTop />
  </div>

  <div id="como-funciona">
    <HowWorks />
  </div>

  <Experience />
  <div id="contact">
     <Contat />
  </div>
  <Footer />
</template>


<style scoped>
.container {
  position: relative;
  width: 100%;
  min-height: 100vh;
}

.scope-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 10;
  pointer-events: auto;
}

</style>