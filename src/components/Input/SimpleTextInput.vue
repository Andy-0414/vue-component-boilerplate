<template>
	<input class="simpletextinput" v-on="$listeners" />
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class SimpleTextInput extends Vue {}
</script>

<style lang="scss">
.simpletextinput {
	border: none;
	background: none;
	outline: none;

	border: 1px solid #36afff;
	color: #36afff;

	border-radius: 10px;

	padding: 10px;

	transition: 0.2s;
}
</style>
