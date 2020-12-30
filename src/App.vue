<template>
  <div id="app">
  	<Blocks />
  </div>
</template>

<script>
import Blocks from '@/components/Blocks'

export default {
  name: 'App',
  components: {
  	Blocks
  }
}
</script>

<style lang="scss">
#app {
	font-family: 'Arial', "Helvetica Neue", 'Helvetica', sans-serif;
}
</style>