<template>
  <div>
    <section class="hero is-primary">
      <div class="hero-body">
        <div class="container">
          <h1 class="title">
            Available themes
          </h1>
          <GalleryThumbnails/>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import GalleryThumbnails from '@/components/GalleryThumbnails';

export default {
  name: 'Gallery',
  data() {
    return {
    };
  },

  components: {
    GalleryThumbnails
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
