<template>
  <v-layout>
    <v-flex class="text-center">
      <div>
        問題リスト
      </div>
      <v-spacer />
      <v-card
        color="primary"
        class="mx-auto"
        max-width="400"
        tile
      >
        <v-list rounded>
          <v-list-item to="/part1">
            <v-list-item-content>
              <v-list-item-title>Part1</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item to="/part2">
            <v-list-item-content>
              <v-list-item-title>Part2</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item to="/part2">
            <v-list-item-content>
              <v-list-item-title>Part3</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-card>
    </v-flex>
  </v-layout>
</template>
