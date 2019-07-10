<template>
  <div>
    <h1>{{title}}</h1>
    <child @getMessage="showMsg"></child>
  </div>
</template>

<script>
  import Child from '../components/child.vue'
  export default {
    components: {Child},
    data(){
      return{
        title:''
      }
    },
    methods:{
      showMsg(title){
        this.title=title;
      }
    }
  }
</script>
