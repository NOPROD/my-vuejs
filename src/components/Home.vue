<template>
  <div class="main_home">
    home
    <div data-relative-input="true" id="scene">
      <div data-depth="0.2">My first Layer!</div>
      <div data-depth="0.6">My second Layer!</div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'
import {} from '@/services'

@Component
export default class Home extends Vue {
  mounted() {
    console.log(this.$i18n)
    setTimeout(() => {
      console.log(this)
    }, 1000)
    // this.initParallax()
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.main_home {
}
</style>

<i18n lang="json5">
{
  "en": {
    "title": {"hi":"hi"
    }
  },
  "fr": {
    "title": {"hi":"hi"
    }
}
}
</i18n>
