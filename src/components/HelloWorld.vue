<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  <p v-if="IsMorning">Good morning!</p>
  <p v-if="isAfterNoon">Good afternoon!</p>
  <p v-if="Isnight">Good evening!</p>
  <p>{{isAfterNoon}} </p>
  <p>{{hour}} </p>
  <p> Page Open Sience {{Seconds}}</p>
  <li v-for="dog in dogs">{{dog}}</li>
  <button v-bind:disabled="buttonDisabled">Test button</button>
    <button v-bind:disabled="buttonEnabled">Test button</button>

  
    <h2>Essential LinksffS</h2>
    <ul>
      <li>
        <a
          href="https://vuejs.org"
          target="_blank"
        >
          Core Docs
        </a>
      </li>
      <li>
        <a
          href="https://forum.vuejs.org"
          target="_blank"
        >
          Forum
        </a>
      </li>
      <li>
        <a
          href="https://chat.vuejs.org"
          target="_blank"
        >
          Community Chat
        </a>
      </li>
      <li>
        <a
          href="https://twitter.com/vuejs"
          target="_blank"
        >
          Twitter
        </a>
      </li>
      <br>
      <li>
        <a
          href="http://vuejs-templates.github.io/webpack/"
          target="_blank"
        >
          Docs for This Template
        </a>
      </li>
    </ul>
    <h2>Ecosystem</h2>
    <ul>
      <li>
        <a
          href="http://router.vuejs.org/"
          target="_blank"
        >
          vue-router
        </a>
      </li>
      <li>
        <a
          href="http://vuex.vuejs.org/"
          target="_blank"
        >
          vuex
        </a>
      </li>
      <li>
        <a
          href="http://vue-loader.vuejs.org/"
          target="_blank"
        >
          vue-loader
        </a>
      </li>
      <li>
        <a
          href="https://github.com/vuejs/awesome-vue"
          target="_blank"
        >
          awesome-vue
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
    created() {
    setInterval(() => {
    this.Seconds++;
}, 1000);
},

  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      isAfterNoon:true,
      IsMorning:true,
      Isnight:false,
      hour: new Date().getHours(),
      dogs :['pit pull','german','husky'],
      buttonDisabled:true,
      buttonEnabled:false,
      Seconds:1
    }

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
