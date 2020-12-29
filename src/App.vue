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

	.container {
		max-width: 1080px;
		margin: 0 auto;
		width: 100%;
		text-align: center;
	}
}
</style>