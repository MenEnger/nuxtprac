<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <div class="text-center" />
      <v-card class="text-center">
        <v-card-title class="headline">
          テストアプリ
        </v-card-title>

        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/list"
          >
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>

export default {
  components: {
  }
}
</script>
