<template>
  <div class="card" @click="openTheme(item)">
    <div class="card-image">
      <figure class="image is-4by3">
        <img :src="'https://vue-git-cms-templates.github.io/' + item.repoUrl + '/preview/thumb.png'" :alt="item.title"/>
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

  methods: {
    openTheme(item) {
      console.log('openTheme', item);
      this.$emit('onOpenTheme', item);
    },
  }
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
