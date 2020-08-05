<template>
	<input class="neumorphismtextinput" v-on="$listeners" />
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class NeumorphismTextInput extends Vue {}
</script>

<style lang="scss">
.neumorphismtextinput {
	cursor: pointer;
	border: none;
	background: none;
	outline: none;

	color: black;

	border-radius: 20px;
	box-shadow: 10px 10px 20px #d9d9d9, -10px -10px 20px #ffffff;

	padding: 10px;

	transition: 0.2s;
	&:hover {
	}
}
</style>
