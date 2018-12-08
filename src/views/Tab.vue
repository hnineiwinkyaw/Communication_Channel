<template>
  <div class="reset">
    <FAB class="FAB"/>
    <md-tabs md-alignment="fixed">


      <md-tab id="tab-home" md-label="News" > <NewFeeds/></md-tab>
      <md-tab id="tab-pages" md-label="Groups"><Groups/></md-tab>
    </md-tabs>
  </div>
</template>

<script>
  import NewFeeds from '@/components/newfeeds.vue'
    import Groups from '@/components/group.vue'
    import FAB from '@/components/fab.vue'
  export default {
    name: 'TabAlignments',
    components: {
    NewFeeds,
    Groups,
    FAB
  }
  }
</script>

<style lang="scss" scoped>
.FAB{
  z-index:1;
}
  .md-tabs {
    margin-bottom: 24px;
  }
  .reset{
    padding: 0px;
  }

</style>