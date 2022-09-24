<template>
  <div class="Home">
    <v-toolbar class="mt-5" flat>
      <v-toolbar-title>
        <span class="caption">总看板</span><br />趋势图
      </v-toolbar-title>
      <v-app-bar flat color="rgba(0,0,0,0)" class="ml-13">
        <v-tabs v-model="tab" color="purple" slider-size="3">
          <v-tab>
            <v-btn fab color="purple lighten-4" elevation="0">
              <v-icon color="purple">fab fa-bitcoin</v-icon>
            </v-btn>
          </v-tab>
          <v-tab>
            <v-btn fab color="red lighten-4" elevation="0">
              <v-icon color="red">fab fa-rupee-sign</v-icon>
            </v-btn>
          </v-tab>
          <v-tab>
            <v-btn fab color="blue lighten-4" elevation="0">
              <v-icon color="green"> fas fa-yen-sign </v-icon>
            </v-btn>
          </v-tab>
          <v-tab>
            <v-btn fab color="grey lighten-4" elevation="0">
              <v-icon color="grey"> fas fa-chevron-right </v-icon>
            </v-btn>
          </v-tab>
        </v-tabs>
      </v-app-bar>
      <v-space>xxx</v-space>
      <v-btn icon>
        <v-icon>far fa-bell</v-icon>
      </v-btn>
      <v-badge bordered bottom color="green" dot offset-x="10" offset-y="10">
      </v-badge>
    </v-toolbar>
  </div>
</template>

<script>
export default {
  name: 'Home',

  data: () => ({
    tab: null,
    text: 'center',
    fill: true,
    padding: 8,
    radius: 10,
    value: [0, 2, 5, 9, 5, 10, 3, 5, 0, 0, 1, 8, 2, 9, 0],
    width: 2,
    lineCap: 'round',
    type: 'trend',
    autoLineWidth: false,
    fills: false,
  }),
}
</script>

<style lang="sass" scoped>
.v-card.on-hover.theme--dark
  background-color: rgba(#FFF, 0.8)
  >.v-card__text
    color: #000
</style>
<style scoped>
.border {
  border-right: 1px solid grey;
}
</style>
