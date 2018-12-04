<template>
  <div>
    <md-card v-for="i in data">
     

        <md-avatar class="ava">
      <img v-bind:src="i.img" alt="Avatar">
    </md-avatar>
        <div class="date">{{i.date}}</div>
        <md-card-header-text class="title">
          <div >{{i.title}}</div>
          <b>{{i.name}}</b>
                 </md-card-header-text>
         
      
      <md-card-content class="content">
        {{i.content}}
      </md-card-content>
     
      <md-card-actions>
        <md-button>Comment</md-button>
      </md-card-actions>
     
    </md-card>

    
  </div>
</template>

<style lang="scss" scoped>
  .md-card {
    width: 320px;
    margin: 4px;
    display: inline-block;
    vertical-align: top;
  }
  .content{
    clear:both;
  }
  .date{
    color:rgba(255,255,255,0.5);
    float:right;
    margin:3px;
 

  }
  .name{float:left;}
  .ava{
    float:left;
    margin:3px;
  }
  .title{
  float:left;
  margin-left:10px;
  }
</style>

<script>
export default {
  name: 'NewFeeds',
  props: {
    msg: String
  },
  data:function(){
   return{
      
      data:[
      
         {
           title:'Team-Groot',
           name:'sawkyaw123',
           content:'Hello I am Saw Kyaw Walar Htwe',
           date:'29.11.2018',
           img:'https://pmcvariety.files.wordpress.com/2015/07/naruto_movie-lionsgate.jpg?w=1000'
        },
         {
           title:'Pre-Phoenix',
           name:'sawkyaw',
          content:'Good Morning',
          date:'1.12.2018',
          img:'https://imgix.ranker.com/user_node_img/50036/1000707993/original/we-both-want-the-same-thing-photo-u1?w=650&q=50&fm=jpg&fit=crop&crop=faces'

         }
       ]
     }
   }
}
</script>