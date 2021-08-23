<template>
  <div id="home">
    <h1>チーム一覧</h1>
    <router-link :to="`/about/${teama}`">{{teama}}</router-link><br>
    <router-link :to="`/about/${teamb}`">{{teamb}}</router-link><br>
    <router-link :to="`/about/${teamc}`">{{teamc}}</router-link><br>
    <router-view></router-view>
  </div>

</template>

<script>
 export default {
  data() {
    return {
      teama: "Team_A",
      teamb: "Team_B",
      teamc: "Team_C",
    };
  }
 };
</script>

<style scoped>
div {
  line-height: 30px;
}
</style>
