<template>
  <div>
    <span v-for="i in items">
      <GalleryThumbnail :item="i"/>
    </span>
  </div>
</template>

<script>
import GalleryThumbnail from '@/components/GalleryThumbnail';

export default {
  name: 'GalleryThumbnails',
  data() {
    return {
      items: [
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
        {title: 'cafe-home', repoUrl: 'https://github.com/vue-git-cms-templates/cafe-home'},
      ],
    };
  },

  components: {
    GalleryThumbnail
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
