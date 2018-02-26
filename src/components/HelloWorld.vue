<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <msg-box @changed="updateMsg"></msg-box>
  </div>
</template>

<script>
import MsgBox from './msgBox'
export default {
  name: 'HelloWorld',
  components: { MsgBox },
  data () {
    return {
      msg: 'Welcome to my Vue.js App'
    }
  },
  methods: {
    updateMsg (value) {
      if (value) {
        this.msg = value
      } else {
        this.msg = 'Welcome to my Vue.js App'
      }
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
