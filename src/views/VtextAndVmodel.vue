<script>
export default{
  data(){
    return{
      title:"title",
      info:{
        name:"可口可樂",
        age:2,
        type:"臘腸"
      },
      cool:""
    }
  }
}
</script>

<template>
  <!-- this不加有可以，只是單純告訴自己this可以指過去 -->
  <h1>{{this.title}}</h1>
  <!-- v-text -->
  <p v-text="title"></p>
  <p v-text="info"></p>
  <p v-text="`info ${title}`"></p>
  <p v-text="'info' + info"></p>
  <p v-text="`info` + info"></p>
  <p>info{{ this.info }}</p>

  <!-- v-model (雙向綁定) -->
  <h2>V-model</h2>
  <input type="text" v-model="cool">
  <p>{{this.cool}}</p>
</template>

<style scoped lang="scss">

</style>
