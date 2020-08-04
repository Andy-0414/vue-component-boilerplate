<template>
	<div id="app">
		<div>
			<h2>SimpleButton</h2>
			<SimpleButton>Hello World</SimpleButton>
		</div>
		<div>
			<h2>SimpleTextInput</h2>
			<SimpleTextInput></SimpleTextInput>
		</div>
	</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import SimpleButton from "./components/Button/SimpleButton.vue";
import SimpleTextInput from "./components/Input/SimpleTextInput.vue";

@Component({
	components: {
		SimpleButton,
		SimpleTextInput,
	},
})
export default class App extends Vue {}
</script>

<style lang="scss">
* {
	margin: 0;
	padding: 0;

	box-sizing: border-box;
}
</style>
