<template>
<h1>
Test Template
</h1>
</template>

<script>
export default {
  name: 'HelloWorldone',
  hour: new Date().getHours(),

  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      isAfterNoon:true,
      IsMorning:true,
      Isnight:false
    }
  }
}
</script>