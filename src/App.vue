<template>
	<div id="app">
		<div class="example">
			<h2>SimpleButton</h2>
			<SimpleButton style="width:100%;">등록하기</SimpleButton>
		</div>
		<div class="example">
			<h2>SimpleCircleButton</h2>
			<SimpleCircleButton style="width:100%;">로그인</SimpleCircleButton>
		</div>
		<div class="example">
			<h2>SimpleInput</h2>
			<SimpleInput placeholder="제목" style="width:100%;"></SimpleInput>
		</div>
		<div class="example">
			<h2>SimpleSearchInput</h2>
			<SimpleSearchInput style="width:100%;"></SimpleSearchInput>
		</div>
		<div class="example">
			<h2>SimpleTextarea</h2>
			<SimpleTextarea style="width:100%;"></SimpleTextarea>
		</div>
	</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import SimpleButton from "./components/SimpleButton.vue";
import SimpleInput from "./components/SimpleInput.vue";
import SimpleSearchInput from "./components/SimpleSearchInput.vue";
import SimpleTextarea from "./components/SimpleTextarea.vue";
import SimpleCircleButton from "./components/SimpleCircleButton.vue";

@Component({
	components: {
		SimpleButton,
		SimpleCircleButton,
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
	font-family: "Noto Sans KR", sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
}
body {
	display: flex;
	justify-content: center;
}
#app {
	font-size: 1.2rem;
	width: 480px;

	border: 1px solid $primary-color;
}
.example {
	width: 100%;
	padding: 20px;
	h2 {
		margin-bottom: 20px;

		color: $primary-color;
	}
}
</style>
