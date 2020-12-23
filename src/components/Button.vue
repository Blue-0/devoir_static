<template>
  <a class="button">
    <slot/> ❯
  </a>
</template>

<script>
import Button from '@/components/Elements/Button'

export default {
  components: {
    Button
  },
  data() {
    return {
      settings: require("../../data/theme.json")
    }
  }
}
</script>

<style>
.button {
  display: inline-block;
  text-transform: uppercase;
  text-decoration: none;
  padding: .75em 1em;
  border-radius: 20px;
}
.is-dark {
  background: black;
  color: white;
}
</style>