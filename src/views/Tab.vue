<template>
  <div class="reset">
    <md-tabs md-alignment="fixed">
      <md-tab id="tab-home" md-label="News" ></md-tab>
      <md-tab id="tab-pages" md-label="Groups"></md-tab>
    </md-tabs>
  </div>
</template>

<script>
  export default {
    name: 'TabAlignments'
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