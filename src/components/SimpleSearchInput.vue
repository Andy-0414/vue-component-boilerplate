<template>
	<div class="simplesearchinput">
		<i class="material-icons search__icon">search</i>
		<input v-on="$listeners" v-bind="$props" />
		<i class="material-icons">cancel</i>
	</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
@Component
export default class SimpleSearchInput extends Vue {}
</script>

<style lang="scss">
.simplesearchinput {
	display: flex;
	align-items: center;

	background-color: $focus-color;

	border-radius: 20px;
	padding: 15px;
	transition: 0.2s;
	i {
		color: $icon-color;
	}
	.search__icon {
		margin-right: 10px;
	}
	input {
		flex: 1;

		border: none;
		background: none;
		outline: none;

		font-size: 1em;
	}
}
</style>
