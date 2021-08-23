<template>
  <div class="about">
    <h1>current team:{{team}}</h1>
    <button @click="counter">counter</button>
    <p>{{ $store.state.count }}</p>
    <p>Last team name cliked:{{team}}</p>
    <router-link to="/">戻る</router-link>
  </div>
</template>


<script>
export default {
  methods:{
    counter(){
      this.$store.commit('counterMutation');
    }
  },
  props: ['team']
}
</script>