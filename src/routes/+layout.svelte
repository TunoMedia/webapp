<script lang="ts">
	import { setWalletProviderContext } from '$lib/Wallet/WalletProviderContext.svelte';
	import { setMusicPlayerContext } from '$lib/Player/MusicPlayer.svelte';
	import '../app.css';

	let { children } = $props();

	setWalletProviderContext();
	setMusicPlayerContext();
</script>

{@render children()}
