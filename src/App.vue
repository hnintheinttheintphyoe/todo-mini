<template>
  <div id="app" class="m-5">
    <MyTitle></MyTitle>
    <ul class="list-group">
      <MyList></MyList>
      <MyList></MyList>
      <MyList></MyList>

    </ul>
    <ul class="list-group mt-3">
      <MyList></MyList>
      <MyList></MyList>
      <MyList></MyList>

    </ul>

  </div>
</template>

<script>
import MyList from './components/MyList.vue'

import MyTitle from './components/MyTitle.vue'

export default {
  name: 'App',
  components: { MyTitle, MyList}
}
</script>

<style>

</style>
