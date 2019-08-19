<template lang="html">
  <v-app>
    <div>
    <img id = "logo" src="~/assets/Logo_namedYule.png" v-on:click="go_home" />
    </div>
    <nav>
      <v-toolbar dark color="blue">
        <v-spacer>
        </v-spacer>
        <v-toolbar-items>
          <v-text-field label = "검색" hide-details prepend-icon="mdi-magnify" :style="{ display: 'flex', alignItems: 'center' }"/>
          <v-btn text nuxt to = "/profile" :style="{ display: 'flex', alignItems:'center' }">
            <div>재고 확인</div>
          </v-btn>
          <v-btn text nuxt to = "/signup">
            <div>재고 검색</div>
          </v-btn>
        </v-toolbar-items>
      </v-toolbar>
    </nav>
    <nuxt/>
  </v-app>
</template>

<script>
export default {
}
</script>

<style lang="css" scoped>
  #logo{
    display: flex;
    align-items: center;
    left : 50%;
    transform: translate(-50%, 0);
    height:6em;
    position: relative;
  }
</style>
