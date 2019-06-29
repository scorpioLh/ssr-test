<template>
  <div>
    <h2>商品列表</h2>
    <ul>
      <li v-for="item in list" :key="item.id">
        <nuxt-link :to="'/detail/' + item.id">{{item.name}}</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data () {
    return {
      list: [
        {
          id: '001',
          name: 'iphone100',
          price: 20000
        },
        {
          id: '002',
          name: 'huawei10000',
          price: 3333
        },
        {
          id: '003',
          name: 'chuizi10001',
          price: 6666
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>


