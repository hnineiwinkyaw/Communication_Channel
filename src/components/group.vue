<template>
  <div >
    <md-list>
   <md-list-item v-for="i in data" href="https://google.com" target="_blank">
     <h5>{{i.group}}</h5>
       <span class="text">{{i.some_text}}</span>
     <span class="date">{{i.date}}</span>
   </md-list-item>
 </md-list>

    
  </div>
</template>

<style lang="scss" scoped>
h5{
  margin-top:-5px;
}
.text{
  margin-top:30px;
  margin-left:-300px;
  float:left;
  color:rgba(225,225,225,0.5);
 
}
  span{
    font-size:0.8em;
  }
  .date{
    color:rgba(225,225,225,0.5);
    
  }
  
</style>

<script>
export default {
  name: 'Groups',
  props: {
    msg: String
  },
  data:function(){
   return{
      
      data:[
     {
      group:'Admin Team',
      some_text:'some text here',
      date:'4:00pm'

     },
     {
      group:'Groot Team',
      some_text:'some text here',
      date:'8:30pm'

     }
       ]
     }
     }
   }

</script>