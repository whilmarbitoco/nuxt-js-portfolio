<template>
	<div>
	<Homepage />
  <Projects />
	</div>
</template>

<script>
export default {
  name: 'IndexPage',
  head() {
    return {
      title: 'Whilmar Bitoco | Front-End Web Developer',
      meta: [
        { hid: 'description', name: 'description', content: 'Welcome to my portfolio.' }
      ]
    }
  }
}
</script>
