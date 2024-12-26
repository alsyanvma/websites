<template>
    <div>
      <navbar />
      <slot />
      <Footer />
      <Gallery />
    </div>
  </template>
  
  <script>
  import Footer from '~/components/footer.vue';
  
  export default {
    components: {
      Footer,
    },
  };
  </script>
  