<template>
  <div>
    <p>{{$store.state.count}}</p>
    <button @click="$store.commit('add')">+1</button>
    <hr />
    <p>{{$store.state.subcount.scount}}</p>
    <button @click="$store.commit('subcount/addScount')">+1</button>
  </div>
</template>

<script>
export default {
  created() {
    console.log(this.$store.state)
  }
}
</script>

