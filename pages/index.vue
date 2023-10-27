<script setup lang="ts">
  const route = useRoute();
</script>

<template>
  <div class="container">
    <nav>
      <ul>
        <li><NuxtLink to="/Home" class="pageLink">Home</NuxtLink></li>
        <li><NuxtLink to="/Tasks" class="pageLink">Tasks</NuxtLink></li>
        <li><NuxtLink to="/Calendar" class="pageLink">Calendar</NuxtLink></li>
        <li><NuxtLink to="/Gallery" class="pageLink">Gallery</NuxtLink></li>
      </ul>
    </nav>
  </div>
  <NuxtPage />
</template>

<style scoped>
html {
  background-color: rgb(213, 218, 209);
}

button {
  font-weight: bold;
}
.container {
  display: flex;
  flex-direction: column;
  align-items: left;
  justify-content: space-around;
  height: 100vh;
  padding-left: 20%;
}
.pageLink{
  text-decoration: none;
  color: rgb(246, 181, 203);
}

.pageLink:hover {
  color: black;
  font-size: 60px;
}
li {
  list-style-type: none;
  margin: 0;
  padding: 0;
  margin-right: 20px;
  font-weight: bold;
  font-size: 48px;
}

</style>