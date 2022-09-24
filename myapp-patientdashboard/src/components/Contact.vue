<template>
  <v-card color="white" class="round-lg mt-2" flat>
    <v-row>
      <v-col cols="12" sm="4">
        <v-card color="#2784ff" class="rounded-lg px-2" flat>
          <v-row>
            <v-col cols="12" sm="4">
              <v-avatar color="#dfedff" tile>
                <v-img src="p1.png"></v-img>
              </v-avatar>
            </v-col>
            <v-col cols="12" sm="8">
              <h4 class="white--text">姓名：{{ name }}</h4>
              <h6 class="white--text">年龄：{{ age }}岁</h6>
            </v-col>
            <v-col cols="12" sm="12" class="mt-3">
              <v-row>
                <v-col cols="12" sm="4">
                  <h6 class="grey--text text--lighten-4">height</h6>
                  <h6 class="white--text">{{ height }}</h6>
                </v-col>
                <v-col cols="12" sm="4">
                  <h6 class="grey--text text--lighten-4">height</h6>
                  <h6 class="white--text">{{ height }}</h6>
                </v-col>
                <v-col cols="12" sm="4">
                  <h6 class="grey--text text--lighten-4">height</h6>
                  <h6 class="white--text">{{ height }}</h6>
                </v-col>
              </v-row>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
      <v-col cols="12" sm="3">
        <v-card color="transparent" class="rounded-lg mx-2 px-2" flat>
          <span class="caption grey--text mt-n6">电话号码</span>
          <h5 class="black--text mb-7">188 888 88888</h5>
          <span class="caption grey--text"> 病历卡号</span>
          <h5 class="black--text">1111111</h5>
        </v-card>
      </v-col>
      <v-col cols="12" sm="5">
        <v-card color="transparent" class="rounded-lg mx-2 px-2" flat>
          <span class="caption grey--text mt-n6">邮箱</span>
          <h5 class="black--text mb-7">1111@ddd.com</h5>
          <span class="caption grey--text"> 疾病诊断</span>
          <h5 class="black--text">过敏,气喘,冠状动脉心脏病</h5>
        </v-card>
      </v-col>
    </v-row>
  </v-card>
</template>

<script>
export default {
  data: () => ({
    name: "kk",
    age: "38",
    height: "185",
  }),
};
</script>

<style></style>
