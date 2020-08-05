<template>
	<button class="neumorphismbutton" v-on="$listeners">
		<slot></slot>
	</button>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class NeumorphismButton extends Vue {}
</script>

<style lang="scss">
.neumorphismbutton {
	cursor: pointer;
	border: none;
	background: none;
	outline: none;

	color: black;

	border-radius: 10px;
	box-shadow: 10px 10px 20px #d9d9d9, -10px -10px 20px #ffffff;

	padding: 10px;

	transition: 0.2s;
	&:hover {
	}
}
</style>
