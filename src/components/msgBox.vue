<template>
    <div class="wrap">
        <input type="text" v-model="msg" placeholder="Entrez un message ici ..." @keyup.enter="changed" />
        <input type="button" value="OK" @click="changed">
        <input type="button" value="Reset" @click="reset">
    </div>
</template>

<script>
export default {
  name: 'MsgBox',
  data () {
    return {
      msg: ''
    }
  },
  methods: {
    changed () {
      this.$emit('changed', this.msg)
    },
    reset () {
      this.msg = ''
      this.changed()
    }
  }
}
</script>

<style scoped>
.wrap {
  text-align: center;
  margin-top: 3em;
}
.wrap input[type="text"] {
  width: 50%;
}
.wrap input[type="button"] {
  width: 10%;
  margin-left: 1em;
}
</style>
