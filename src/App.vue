<script>
export default {
  data() {
    return {
      name: 'Hashi car Sales',
      status: 'pending',
      tasks: ['task one', 'Task two', 'Task three'],
      link: 'https://google.com'
    };
  },
  methods: {
    toggleStatus() {
      if (this.status == 'active') {
        this.status = 'pending';
      } else if (this.status == 'pending') {
        this.status = 'inactive';
      } else {
        this.status = 'active';
      }
    }
  }
}
</script>

<template>
  <h1>{{ name }}</h1>
  <br>
  <p v-if="status == 'active'">User is active</p>
  <p v-else-if="status == 'pending'">User is pending</p>
  <p v-else>User is inactive</p>
<br>
  <h3>Tasks:</h3>
  <br>
  <ul>
    <li v-for="task in tasks" :key="Tasks">{{ task }}</li>
  </ul>
  <br>
  <!--a v-bind:href="link">Click for google!</a-->
  <a :href="link">Click for Google</a>
  <br>
  <!--button v-on:click="toggleStatus">Change status</button-->
  <button @click="toggleStatus">Change status</button>
</template>
