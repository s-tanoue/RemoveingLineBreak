<template>
  <div>
    <v-textarea
      v-model="text"
      name="input-7-1"
      label=" Please paste the sentence you want to remove the line break"
    />
    <v-btn @click="resharpe">
      Removed line breaks
    </v-btn>
  </div>
</template>

<script>

export default {
  components: {
  },
  data () {
    return {
      text: ''
    }
  },
  methods: {
    resharpe () {
      this.text = this.text.replace(/\r?\n/g, ' ')
    }
  }
}
</script>
