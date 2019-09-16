<template>
  <div class="jumbotron">
    <h1>This is a jumbotron</h1>
    <ul>
      <list-item
        v-for="item in items"
        v-bind:item="item"
        v-bind:key="item.id"
      ></list-item>
    </ul>
  </div>
</template>

<script>
// @ is an alias to /src
import ListItem from '@/components/ListItem.vue'

export default{
  name: 'jumbo',
  components: {
    ListItem
  },
  data(){
    return {
      items:[{id:1,text:'One'},{id:2,text:'Two'},{id:3,text:'Three'}]
    }
  }
}
</script>
