<template>
    <Navbar/>
    <Index/>
    <Footer/>
</template>

<script>
import Navbar from "./views/allviews/Navbar.vue";
import Footer from "./views/allviews/Footer.vue";
import Index from "./components/home/Index.vue";
export default {
  components: {
    Navbar,
    Footer,
    Index
  },
};
</script>