<template>
<div class="jmgmzlwq _block"><i class="fas fa-exclamation-triangle" style="margin-right: 8px;"></i>{{ $ts.remoteUserCaution }}<a :href="href" rel="nofollow noopener" target="_blank">{{ $ts.showOnRemote }}</a></div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import * as os from '@/os';

export default defineComponent({
	props: {
		href: {
			type: String,
			required: true
		},
	},
	data() {
		return {
		};
	}
});
</script>

<style lang="scss" scoped>
.jmgmzlwq {
	font-size: 0.8em;
	padding: 16px;
	background: var(--infoWarnBg);
	color: var(--infoWarnFg);

	> a {
		margin-left: 4px;
		color: var(--accent);
	}
}
</style>
