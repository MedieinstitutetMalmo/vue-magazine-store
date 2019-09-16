<template>
  <li>{{item.text}}</li>
</template>

<script>
export default {
  name: 'ListItem',
  props: ['item']
}
</script>