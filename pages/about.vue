<template>
  <v-row>
    <v-col>
      <blockquote class="blockquote">{{aboutText}}</blockquote>
    </v-col>
  </v-row>
</template>

<style scoped>
  blockquote {
    background: url('@/static/left_widget_img.jpg');
    background-size: cover;
  }
</style>

<script>
export default {
  name: 'InspirePage',
  computed: {
    aboutText() {
      return this.$store.getters.aboutText;
    }
  }
}
</script>
