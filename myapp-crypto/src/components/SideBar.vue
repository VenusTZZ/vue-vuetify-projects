<template>
  <v-navigation-drawer v-model="drawer" permanent color="#F4F5F9" app>
    <v-list-item class="px-2 py-5">
      <v-list-item-title class="text-capitalize" align="center">
        <v-icon> fab fa-bitcoin </v-icon>
        乌龙币
      </v-list-item-title>
    </v-list-item>
    <v-list>
      <v-list-item-group v-model="selectedItem" color="deep-purple">
        <v-list-item v-for="(item, i) in items" :key="i">
          <v-list-item-icon>
            <v-icon> {{ item.icon }} </v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title> {{ item.text }} </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list-item-group>
    </v-list>

    <template v-slot:append>
      <div class="pa-2">
        <v-card align="center" class="pa-3">
          <v-badge
            bordered
            bottom
            color="green"
            dot
            offset-x="10"
            offset-y="10"
            class="mb-8"
          >
            <v-avatar size="40">
              <v-img src="https://cdn.vuetifyjs.com/images/lists/2.jpg"></v-img>
            </v-avatar>
          </v-badge>
          <h4 class="grey--text">我的账户</h4>
          <h2>$852.50</h2>
          <h5 class="green--text">今日新增:￥583.4</h5>
          <v-card color="deep-purple" dark class="mt-5">
            <v-list-item two-line>
              <v-list-item-content>
                <v-list-item-title> 钱包地址: </v-list-item-title>
                <v-list-item-subtitle> 3jnkb1lj49jklj </v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
          </v-card>
        </v-card>
      </div>
    </template>
  </v-navigation-drawer>
</template>
<script>
export default {
  name: 'SideBar',
  data: () => ({
    //
    selectedItem: 0,
    drawer: null,
    items: [
      { icon: 'fas fa-home', text: '看板', route: '/home' },
      {
        icon: 'fas fa-money-check-alt',
        text: '买入 / 卖出',
        route: '/hobuysme',
      },
      { icon: 'fas fa-dolly', text: '业务', route: '/transactions' },
      { icon: 'fas fa-exchange-alt', text: ' 兑换', route: '/exchanges' },
      { icon: 'fas fa-cog', text: '工具', route: '/tools' },
    ],
  }),
  components: {
    //
  },
}
</script>
<style scoped>
div >>> .v-list a {
  text-decoration: none;
}
</style>
