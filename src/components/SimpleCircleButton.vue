<template>
	<button class="simplecirclebutton" v-on="$listeners" v-bind="$props">
		<slot></slot>
	</button>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
@Component
export default class SimpleCircleButton extends Vue {}
</script>

<style lang="scss">
.simplecirclebutton {
	cursor: pointer;
	border: none;
	background: none;
	outline: none;

	background-color: $primary-color;
	color: white;

	font-size: 1em;
	font-weight: bold;

	border-radius: 100px;
	padding: 15px;
	transition: 0.2s;

	&:hover {
		filter: brightness(1.1);
	}
	&:active {
		filter: brightness(0.9);
	}
}
</style>
