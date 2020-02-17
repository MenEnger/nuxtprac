<template>
  <v-layout class="container">
    <v-flex class="text-center">
      <div>
        <p>Part1</p>
        <p>
          横断歩道では、渡る人が待っている場合は残らなければならない
        </p>
        <v-btn
          color="red"
          nuxt
          to="/part1ans"
        >
          ○
        </v-btn>
        <v-btn
          color="blue"
          nuxt
          to="/part1ans"
          style="margin-left:10px"
        >
          ×
        </v-btn>
      </div>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  // Called to know which transition to apply
  transition (to, from) {
    return 'slide-left'
  }
}
</script>

<style>
.container {
  transition: all 1s ease-out;
}
.slide-left-enter,
.slide-right-leave-active {
  opacity: 0;
  transform: translate(30px, 0);
}
.slide-left-leave-active,
.slide-right-enter {
  opacity: 0;
  transform: translate(-30px, 0);
}
</style>
