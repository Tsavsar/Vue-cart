<script setup>
  import { ref } from 'vue';
import Childcomponent from './components/childcomponent.vue';


const items = ref([
  { id: 1, name: 'Chicken' },
  { id: 2, name: 'Ice' },
  { id: 3, name: 'Wing' }
])

const posts = ref([
  { id: 1, title: 'My journey with Vue' },
  { id: 2, title: 'Blogging with Vue' },
  { id: 3, title: 'Why Vue is so fun' }
])
// const function = item => {

// }






// const message= ref('Hello bro')

// const childMsg = ref('No child msg yet')
  // // const counter = reactive({count: 0})
  // const count = ref(0)

  // function increment(){
  //   count.value++
  // }
  // function dec(){
  //   count.value--
  // }

  // const text= ref ('')

  // const yeat = ref(true)

  // function toggle(){
  //   yeat.value = !yeat.value
  // }

  // const col = ref(true)

  // function change(){
  //   col.value = !col.value
  // }
  // // const message = ref ('hello world')
  // const titleclass = ref ('title')

  // let id = 0

  // const newtodo = ref('')
  // const hidecom = ref(false)
  // const todos= ref([
  //   { id:id++ , text: 'learn JS', done: true},
  //   { id:id++ , text: 'learn Html', done: false},
  //   { id:id++ , text: 'learn CSS', done: false}

  // ])

  // //now we will filter t.done
  // const filteredtodos = computed(() => {
  //   return hidecom.value
  //   ? todos.value.filter((t) => !t.done)
  //   : todos.value
  // })

  // function addtodo(){
  //   todos.value.push({id: id++, text: newtodo.value})
  //   newtodo.value=''
  // }

  // function remove(todo){
  //   todos.value = todos.value.filter((t)=> t !==todo)

//     The filter function filters all the words in the array which have length greater than 5

// var words = ["hi", "hello", "hey", "apple", "watermelon",
//             "lemon", "javascript"];
// var result = words.filter(word => word.length > 5);
// console.log(result);
// Output :

// [ 'watermelon', 'javascript' ]
//   }

// const heartclass = ref('like')

// const heart = ref(false)

// function like(){
//   heart.value = !heart.value
// }
</script>


<template>
<Childcomponent
v-for="post in posts"
:key="post.id"
:title="post.title"
:num="posts.length"/>



<!-- <form @submit.prevent="addtodo()">
  <input v-model="newtodo" type="text">
<button>Add Todo</button>
</form>
<br>
<button @click="heart = !heart">
  <h1 v-if="heart" :class="heartclass">I like this</h1>
<h1 v-else>I don't like this</h1>

</button>


<br>
<ul>
  <li v-for="todo in filteredtodos" :key="todo.id" >
    <input type="checkbox" v-model="todo.done">
    <span :class="{ done: todo.done }">{{ todo.text }}</span>
    <button @click="remove(todo)">X</button>
  </li>
</ul>
<button @click="hidecom = !hidecom">
  {{ hidecom ? 'Show all' : 'Hide com' }}
</button> -->
<!--
<br>
  <br>
<h1 v-if="col" :class="titleclass" > yo bro </h1>
<h1 v-else > yo bro </h1>

<button @click="change">^</button>
<br>
<br>
<p>The Count is: {{counter.count}}</p>
<input v-model="text" placeholder="Type here" type="text">
<br>
<button @click="increment" > the value is : {{count}}</button>
<button @click="dec"> -</button>


<p>{{text}}</p>

<br>
<br>
<br>


<button @click="toggle">toggle</button>
<h1 v-if="yeat" > Yeat makes bangers </h1>
<h1 v-else > Yeat still makes bangers </h1>
 -->

</template>

<style>
  body {
    margin: 0;
    width: 100%;
    height: 100%;
    background-color: #C0E0FF;
    overflow-x: hidden;
    overflow-y: scroll;

    padding: 20px;
    z-index: 0;
  }

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

</style>