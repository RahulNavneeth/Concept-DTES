<script lang="ts">
	const SURFACE_TITLE: string = 'SURFACE';
	let loadingDots: string = '.';
	setInterval(() => {
		if (loadingDots.length === 3) loadingDots = '.';
		else loadingDots += '.';
	}, 500);
</script>

<div
	class="absolute dark:bg-black dark:text-white w-screen h-screen flex flex-col items-center justify-center"
>
	<div class="text-[100px]">{SURFACE_TITLE}</div>
	<span class="text-[25px]">{loadingDots}</span>
</div>
