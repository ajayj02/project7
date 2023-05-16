<template>
  <div>
    <h1 class="heading"
    size="is-medium">Buefy Assignment</h1>
    <Dropdown/>
    <HelloWorld/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Dropdown from './components/Dropdown.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    Dropdown
  }
}
</script>

