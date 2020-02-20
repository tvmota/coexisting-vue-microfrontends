<template>
  <div class="grid__container">
    <header class="grid__container__header">
      <h1>header</h1>
    </header>
    <aside class="grid__container__sidebar">
      <router-link to="/app1">App1</router-link>
      <router-link to="/app2">App2</router-link>
      <router-link to="/app3">App3</router-link>
    </aside>
    <main class="grid__container__content">
      <div id="app1"></div>
      <div id="app2"></div>
      <div id="app3"></div>
    </main>
  </div>
</template>

<style>
.grid__container {
  display: grid;
  grid-template-columns: 200px repeat(4, 1fr);
  grid-template-rows: 80px repeat(4, 1fr);
  grid-column-gap: 0px;
  grid-row-gap: 0px;
  height: 100%;
}

.grid__container__header {
  border: 1px solid #cacaca;
  grid-area: 1 / 1 / 2 / 6;
}
.grid__container__sidebar {
  border: 1px solid #cacaca;
  grid-area: 2 / 1 / 6 / 2;
}
.grid__container__content {
  padding: 8px;
  grid-area: 2 / 2 / 6 / 6;
}
</style>
