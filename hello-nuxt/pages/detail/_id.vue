<template>
  <div>
    <h2>详情页</h2>
    <p>{{$route.params.id}}</p>
    <p>{{detail.price}}</p>
    <p>{{detail.description}}</p>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  asyncData () {
    return axios.get('/data/test.json').then(res => {
      return {
        detail: res.data
      }
    })
  }
}
</script>

