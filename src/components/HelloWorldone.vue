<template>
<div class="hello">
<h1>
Test Templateddd
{{msg}}
</h1>
<h2>
{{msg}}
</h2>
</div>
</template>

<script>
export default {
  name: 'HelloWorldone',
  hour: 300,
  data () {
    return {
      msg: 'Welcome to Your Ve.js App',
      isAfterNoon:true,
      IsMorning:true,
      Isnight:false,
      path :locaton.pathname,
      Seconds:1
    }
  }
}
</script>