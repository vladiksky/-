<template>
  <div id="app">
    <h1>Список дел</h1>
    <div class="tasks-container">
      <TaskItem 
        v-for="task in tasks" 
        :key="task.id" 
        :task="task"
      />
    </div>
  </div>
</template>

<script>
import TaskItem from './components/TaskItem.vue'

export default {
  name: 'App',
  components: {
    TaskItem
  },
  data() {
    return {
      tasks: [
        {
          id: 1,
          title: 'Изучить Vue.js',
          text: 'Пройти базовый курс по Vue.js и изучить основные концепции'
        },
        {
          id: 2,
          title: 'Сделать проект',
          text: 'Создать приложение "Список дел" на Vue'
        },
        {
          id: 3,
          title: 'Изучить компоненты',
          text: 'Разобраться с созданием и использованием компонентов'
        },
        {
          id: 4,
          title: 'Работа с props',
          text: 'Понять как передавать данные между компонентами через props'
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Arial, sans-serif;
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}

.tasks-container {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

h1 {
  text-align: center;
  color: #2c3e50;
  margin-bottom: 30px;
}
</style>

<template>
  <div class="task-item">
    <h3 class="task-title">{{ task.title }}</h3>
    <p class="task-text">{{ task.text }}</p>
  </div>
</template>

<script>
export default {
  name: 'TaskItem',
  props: {
    task: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>
.task-item {
  border: 1px solid #ddd;
  border-radius: 8px;
  padding: 15px;
  background-color: #f9f9f9;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  transition: transform 0.2s ease;
}

.task-item:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.15);
}

.task-title {
  margin: 0 0 10px 0;
  color: #2c3e50;
  font-size: 1.2em;
  font-weight: bold;
}

.task-text {
  margin: 0;
  color: #555;
  line-height: 1.4;
}
</style>
