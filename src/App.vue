<template>
  <div id="app">
    <TodoHeader></TodoHeader>
    <TodoInput></TodoInput>
    <TodoList></TodoList>
    <TodoFooter></TodoFooter>
  </div>
</template>

<script>
//import 불러올 파일의 내용이 담길 객체 from '불러울 파일 위치'
import TodoHeader from './components/TodoHeader.vue'
import TodoInput from './components/TodoInput.vue'
import TodoList from './components/TodoList.vue'
import TodoFooter from './components/TodoFooter.vue'

export default {
  components: {
    'TodoHeader': TodoHeader, //컴포넌트 이름 : 컴포넌트 내용
    'TodoInput': TodoInput,
    'TodoList': TodoList,
    'TodoFooter': TodoFooter
  }
}
</script>

<style >
  body {
    text-align : center;
    background-color : #F6F6F8;
  }

  input {
    border-style : groove;
    width : 200px;
  }

  button {
    border-style : groove;
  }

  .shadow {
    box-shadow : 5px 10px 10px rgba(0, 0, 0, 0.03)
  }
</style>
