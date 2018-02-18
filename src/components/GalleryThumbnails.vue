<template>
  <div>
    <span v-for="i in items">
      <GalleryThumbnail :item="i" @onOpenTheme="openTheme"/>
    </span>
    <b-modal :active.sync="previewModalOpen" :width="640" scroll="keep">
      <div class="card" v-if="previewItem">
        <iframe :src="'https://vue-git-cms-templates.github.io/' + previewItem.title"></iframe>
      </div>
    </b-modal>
  </div>
</template>

<script>
import GalleryThumbnail from '@/components/GalleryThumbnail';

export default {
  name: 'GalleryThumbnails',
  data() {
    return {
      previewModalOpen: false,
      previewItem: undefined,
      items: [
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
        {title: 'cafe-home', repoUrl: 'cafe-home'},
      ],
    };
  },

  methods: {
    openTheme(theme) {
      this.previewModalOpen = true;
      this.previewItem = theme;
    },
  },

  components: {
    GalleryThumbnail
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
iframe {
    width:100%;
    height:500px;
}
</style>
