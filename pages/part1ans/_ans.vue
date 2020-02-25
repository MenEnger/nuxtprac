<template>
  <v-layout>
    <v-flex class="text-center">
      <div>
        <p>Part1</p>
        <div v-if="isCorrect" class="ok">
          ○ 正解
        </div>
        <div v-else class="ng">
          × 不正解
        </div>
        <p>
          横断歩道では、渡る人が待っている場合は残らなければならない
        </p>
        <p>
          横断歩道に人が待っているときは、その人が渡り終えるまで一時停止している必要があります。
        </p>
        <v-btn
          color="primary"
          nuxt
          to="/comp"
        >
          次の問題へ
        </v-btn>
      </div>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  data () {
    // data judge () {
    return { isCorrect: this.$route.params.ans === 'true' }
    // }
  }

}
</script>

<style lang="scss">
.answer {
  font-size: 24px;
  font-weight: bold;
  margin : 8px auto;
}
.ok {
  @extend .answer;
  color: red
}
.ng {
  @extend .answer;
  color: skyblue
}
</style>
