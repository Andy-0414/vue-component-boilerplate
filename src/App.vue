<template>
	<div id="app">
		<div class="example">
			<h2>SimpleButton</h2>
			<SimpleButton>Hello World</SimpleButton>
		</div>
		<div class="example">
			<h2>SimpleInput</h2>
			<SimpleInput></SimpleInput>
		</div>
		<div class="example">
			<h2>SimpleSearchInput</h2>
			<SimpleSearchInput></SimpleSearchInput>
		</div>
		<div class="example">
			<h2>SimpleTextarea</h2>
			<SimpleTextarea></SimpleTextarea>
		</div>
	</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import SimpleButton from "./components/SimpleButton.vue";
import SimpleInput from "./components/SimpleInput.vue";
import SimpleSearchInput from "./components/SimpleSearchInput.vue";
import SimpleTextarea from "./components/SimpleTextarea.vue";

@Component({
	components: {
		SimpleButton,
		SimpleInput,
		SimpleSearchInput,
		SimpleTextarea,
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
.example {
	width: 400px;
	padding: 20px;
	h2 {
		margin-bottom: 20px;

		color: #36afff;
	}
}
</style>
