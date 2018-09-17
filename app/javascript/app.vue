<template lang='pug'>
  #app
    p(v-for="item in ['before', 'sticky', 'enabled']" :key="item") {{ item }}
    nav(style="position: sticky; top: 20px; z-index: 101;")
      ul
        li
          a(href='#') This
        li
          a(href='#') Nav, created in the hello_vue component 
        li
          a(href='#') Wont
        li
          a(href='#') Stick
      p(v-for="item in 100" :key="item") {{ item }}
</template>
<script>
export default {
  data: function () {
    return {
      message: "Hello Vue!"
    }
  }
}
</script>

<style scoped>
nav {
  position: sticky;
  top: 0px;
}
</style>
