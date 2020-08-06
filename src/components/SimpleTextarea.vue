<template>
	<input class="simpletextarea" v-on="$listeners" />
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
@Component
export default class SimpleTextarea extends Vue {}
</script>

<style lang="scss">
.simpletextarea {
	cursor: pointer;
	border: none;
	background: none;
	outline: none;
	border: 1px solid #36afff;
	color: #36afff;
	border-radius: 10px;
	padding: 10px;
	transition: 0.2s;
	&:hover {
		background-color: #36afff;
		color: white;
	}
}
</style>