<script setup>
import Header from "./components/Shared/Header.vue";

import Footer from "./components/Shared/Footer.vue";


import ScrollToTop from "./components/Reusable/ScrollToTop.vue";

</script>

<template className = "container mx-auto" >

  <Header />
  <router-view />
  <ScrollToTop />
  <Footer />
  
</template>

