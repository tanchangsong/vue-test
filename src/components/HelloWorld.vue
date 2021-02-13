<template>
  <div class="hello">
   {{addResult}}

   <p v-if="seen">你好，效力</p>
   <span>修改项</span>
   <!--
   <div id="dooor-test">
     <ol>
      <li v-for="todo in todos">
        {{ todo.text }}
      </li>
    </ol>
  </div> -->
   
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      addResult: 'Welcome to China'+ new Date().toLocaleString(),
      seen: true,
      todos: [
      { text: '学习 JavaScript' },
      { text: '学习 Vue' },
      { text: '整个牛项目' }
    ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
