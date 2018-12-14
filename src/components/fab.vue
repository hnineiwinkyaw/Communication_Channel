<template>
        
        
        <md-speed-dial class="md-bottom-right md-fixed">
          <md-dialog :md-active.sync="showDialog">
             <md-dialog-actions class="md-top-left">
        <md-button class="md-primary " @click="showDialog = false">Close</md-button>
        
      
            <md-button class="md-primary " @click="showDialog = false">Post</md-button>
          </md-dialog-actions>
            <span v-for="i in data">
            <md-avatar  class="ava">
            <img v-bind:src="i.proPic"/>
          </md-avatar>
           <b>{{i.name}}</b>
        </span>
      <md-field class="tex" md-inline>
      <label>Post something?</label>
      <md-textarea v-model="autogrow" md-autogrow></md-textarea>
    </md-field>


      <md-tabs md-dynamic-height>
        
      </md-tabs>
     
      <md-button class="md-fab md-fab-bottom-left md-primary">
        <md-icon md-src="https://image.flaticon.com/icons/svg/1246/1246324.svg ">menu</md-icon>
      </md-button>
      <md-button class="md-fab md-fab-bottom-center md-primary">
        <md-icon md-src="https://image.flaticon.com/icons/svg/1246/1246239.svg">menu</md-icon>
      </md-button>
      <md-button class="md-fab md-fab-bottom-right md-primary">
        <md-icon md-src="https://image.flaticon.com/icons/svg/1244/1244574.svg">menu</md-icon>
      </md-button>
  
    
    </md-dialog>
          <md-speed-dial-target class="md-primary md-accent md-raised" @click="showDialog = true" >
            <md-icon md-src="https://image.flaticon.com/icons/svg/1246/1246321.svg">add</md-icon>
          </md-speed-dial-target>
        </md-speed-dial>
</template>
<style lang="scss" scoped>
.tex{
  width:90%;
  margin:auto;
 background-color: transparent;
    border: 0px solid;
    color: #CCC;
}
.tab{
 margin-bottom:10px;
}
.ava{
    float:left;
    margin:3px;
  }
</style>

<script>
export default {
  name: 'FAB',
     data:function(){
   return{
      showDialog: false,
      data:[
      
         {
           title:'Team-Groot',
           name:'sawkyaw123',
           content:'Hello I am Saw Kyaw Walar Htwe',
           date:'29.11.2018',
           proPic:'https://pmcvariety.files.wordpress.com/2015/07/naruto_movie-lionsgate.jpg?w=1000',
           img:'https://dw9to29mmj727.cloudfront.net/promo/2016/5248-SeriesHeaders_NARSHP_2000x800.jpg'
        
         }
       ]
     }
}
}
</script>