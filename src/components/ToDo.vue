<template>
  <div id="ToDo">
    <h1>Luyen tap Vue</h1>
    <div class="container">
      <div id="tasks">
        <h2> Nhiem Vu Moi </h2>
          <ol class="list-group">
            <li v-for = "(task,index) in tasks" :key="index" class="list-group-item">
              {{task.body}}
            </li>
          </ol>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  el: "#tasks",
  data: function() {
    return {
      tasks: [
              {body:'Di Lam 0',completed: false},
              {body:'Di Lam 1',completed: false},
              {body:'Di Lam 2',completed: false},
              {body:'Di Lam 3',completed: false},
              ]
      
      }
  }
};
</script>