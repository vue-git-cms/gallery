<template>
  <div class="card">
    <div class="card-image">
      <figure class="image is-4by3">
        <img :src="item.repoUrl + 'preview/thumb.png'" :alt="item.title"/>
      </figure>
    </div>
    <div class="card-content">
      <div class="media">
        <div class="media-content">
          {{item.title}}
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'GalleryThumbnail',

  props: ['item'],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.card {
  width: 200px;
  height: 200px;
  display: inline-block;
  float: left;
  margin: 12px;
}

.media-content {
  color: black;
}
.card-content {
  padding: 0.75rem;
}
</style>
