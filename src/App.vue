<template>
<div>
    <h1 class="heading" size="is-medium">Buefy Assignment</h1>
    <div>
        <Sidebar />
    </div>
    <div class="drop">
        <Dropdown />
    </div>

    <div class="Hello">
        <HelloWorld />
    </div>
</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import Dropdown from './components/Dropdown.vue';
import Sidebar from './components/Sidebar.vue';

export default {
    name: 'App',
    components: {
        HelloWorld,
        Dropdown,
        Sidebar
    }
}
</script>

<style>
.Hello {
    margin-top: 15px;
}
</style>
