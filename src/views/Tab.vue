<template>
  <div class="reset">
    <md-tabs md-alignment="fixed">
      <md-tab id="tab-home" md-label="News" ><NewFeeds/></md-tab>
      <md-tab id="tab-pages" md-label="Groups"></md-tab>
    </md-tabs>
  </div>
</template>

<script>
  import NewFeeds from '@/components/newfeeds.vue'
  export default {
    name: 'TabAlignments',
    components: {
    NewFeeds
  }
  }
</script>

<style lang="scss" scoped>
  .md-tabs {
    margin-bottom: 24px;
  }
  .reset{
    padding: 0px;
  }

</style>