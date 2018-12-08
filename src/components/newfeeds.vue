<template>
  <div>
    <md-card v-for="i in data">
     

        <md-avatar class="ava">
      <img v-bind:src="i.proPic" alt="Avatar">
    </md-avatar>
        <div class="date">{{i.date}}</div>
        <md-card-header-text class="title">
          <div >{{i.title}}</div>
          <b>{{i.name}}</b>
                 </md-card-header-text>
         
      <md-card-media class="img">
        <img v-bind:src="i.img">
      </md-card-media>
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
.pos{
  transform:none;
  position:fixed;
}
  .md-card {
    width: 320px;
    margin: 4px;
    display: inline-block;
    vertical-align: top;
  }
  .img {
    clear:both;
    margin:5px;
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
           proPic:'https://pmcvariety.files.wordpress.com/2015/07/naruto_movie-lionsgate.jpg?w=1000',
           img:'https://dw9to29mmj727.cloudfront.net/promo/2016/5248-SeriesHeaders_NARSHP_2000x800.jpg'
        },
         {
           title:'Pre-Phoenix',
           name:'sawkyaw',
          content:'Good Morning',
          date:'1.12.2018',
          proPic:'https://imgix.ranker.com/user_node_img/50036/1000707993/original/we-both-want-the-same-thing-photo-u1?w=650&q=50&fm=jpg&fit=crop&crop=faces',
          img:'https://images.unsplash.com/photo-1530156214126-9e1307659993?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=0dab1d996ed6c8b93ed58760a4a77ce9&w=1000&q=80'

         },
         {
          title:'Pre-Phoenix',
          name:'KyawWalar',
          content:'Help!',
          date:'5.12.2018',
          proPic:'https://images-na.ssl-images-amazon.com/images/I/41BgUB8RcpL.jpg',
          img:''
         }
       ]
     }
   }
}
</script>