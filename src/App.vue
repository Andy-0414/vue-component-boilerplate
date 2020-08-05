<template>
	<div id="app">
		<div class="example">
			<h2>SimpleButton</h2>
			<SimpleButton>Hello World</SimpleButton>
		</div>
		<div class="example">
			<h2>SimpleTextInput</h2>
			<SimpleTextInput></SimpleTextInput>
		</div>
		<div class="example">
			<h2>NeumorphismButton</h2>
			<NeumorphismButton>Hello World</NeumorphismButton>
		</div>
		<div class="example">
			<h2>NeumorphismTextInput</h2>
			<NeumorphismTextInput></NeumorphismTextInput>
		</div>
	</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import SimpleButton from "./components/Button/SimpleButton.vue";
import SimpleTextInput from "./components/Input/SimpleTextInput.vue";
import NeumorphismButton from "./components/Button/NeumorphismButton.vue";
import NeumorphismTextInput from "./components/Input/NeumorphismTextInput.vue";

@Component({
	components: {
		SimpleButton,
		SimpleTextInput,
		NeumorphismButton,
		NeumorphismTextInput,
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
	padding: 40px;
	h2 {
		margin-bottom: 40px;

		color: #36afff;
	}
}
</style>
