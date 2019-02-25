<template>
  <div id="app">

    我的第一个vue程序<br/> 
    {{text}}<br/>
    <input type="text" v-model="text">
    <ul>
      <li v-for="person in list">
        {{person.name}}
      </li>
    </ul>
  <hr/>
  <span v-html="html"></span>
  <hr/>
  v-if:
  <div v-if="isShow" style="height: 100px;background-color: red;"></div>
  <hr/>
  v-show:
  <div v-show="isShow" style="height: 100px;background-color: red;"></div>
  <hr/>
  v-model:
  <input type="text" v-model="mText">
  {{mText}}
  
  <hr/>
  <input type="text" v-bind:value="mText">
  </div>
</template>

<script>

export default {
  name: 'app',
  components: {

  },
  data(){
    return{
      text:'大家好',
      list:[{name:"jack"},{name:"yuheng"}],
      html:`<ul>
        <li>我是猪头三</li>
        <li>我是猪头四</li>
        <li>我是猪头五</li>
      </ul>
      `,
      isShow:true,
      mText:"haha",

    }
  }
}
</script>

<style>
* {
  margin:0;
  padding: 0;
  box-sizing: inherit;
}
#app {
  width: 100vw;
  height: 100vh;
  box-sizing: border-box;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;

}
</style>

