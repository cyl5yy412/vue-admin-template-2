<template>
  <div class="dashboard-container">
    <h1>welcome</h1>
    <br>
    <!-- <div class="dashboard-text">name: {{ name }}</div> -->
    <br>
    <div class="dashboard-text">username: {{ username }}</div>
  </div>
</template>

<script>
//使用vuex 拿到变量
import { mapGetters } from 'vuex'

export default {
  name: 'Dashboard',
  computed: {
    ...mapGetters([
      'name',
      'username',
    ])
  }
}
</script>

<style lang="scss" scoped>
.dashboard {
  &-container {
    margin: 30px;
  }
  &-text {
    font-size: 30px;
    line-height: 46px;
  }
}
</style>
