<!-- pages/projects.vue -->

<template>
  <section class="section is-medium">
    <div class="container has-text-centered">
      <h1 class="title">My Works</h1>
      <ul id="example-1">
        <li v-for="item in items" :key="item.id">
          {{ item.message }}
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
import Vue from 'vue';
  var example1 = new Vue({
  el: '#example-1',
  data: {
    items: [
      { message: 'Foo' },
      { message: 'Bar' }
    ]
  }
});

export default {
  
}
</script>