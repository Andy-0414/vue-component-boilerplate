<template>
	<textarea class="simpletextarea" v-on="$listeners" v-bind="$props" />
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
@Component
export default class SimpleTextarea extends Vue {}
</script>

<style lang="scss">
.simpletextarea {
	border: none;
	background: none;
	outline: none;

	background-color: $nofocus-color;

	font-size: 1em;

	border-radius: 5px;
	padding: 15px;
	transition: 0.2s;
}
</style>
