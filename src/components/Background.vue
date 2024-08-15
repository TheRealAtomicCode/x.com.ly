<template>

	<div class="outter">
		<div class="main">
			<div class="divcontainer">
				<div
					v-for="(item, index) in hexagonCount"
					:id="'id-' + index.toString()"
					:key="index"
					:class="{ hovered: trailIndices.includes(index) }"
					:style="{ backgroundColor: hexagonColors[index] }"
					@mouseenter="handleMouseEnter(index)"
				></div>
			</div>
			890
		</div>
	</div>
</template>

<style>
	.main {

		background-color: #191919;
		position: relative;
		right: 0rem;
		width: 130vw;
		bottom: 0rem;
		display: flex;
		--s: 48px; /* size */
		--m: 0px; /* margin */
		--f: calc(1.732 * var(--s) + 4 * var(--m) - 1px);
	
	}

	.divcontainer {
		font-size: 0; /*disable white space between inline block element */
		background-color: #191919;
	}

	.outter {

		z-index: -2;
		position: absolute;
		width: 110vw;
		overflow: hidden;
		background-color: #191919;
	}

	.divcontainer div {
		width: var(--s);
		 margin: var(--m); 
		height: calc(var(--s) * 1.1547);
		display: inline-block;
		font-size: initial;
		clip-path: polygon(0% 25%, 0% 75%, 50% 100%, 100% 75%, 100% 25%, 50% 0%);
		 background: #191919; 
		margin-bottom: calc(var(--m) - var(--s) * 0.2885);
     margin-right: 1px;
     		transition: background-color 1s;
	}

	.divcontainer div.hovered {
    
		transition: background-color 0s;
	}

	.divcontainer::before {
    
		content: '';
		width: calc(var(--s) / 2 + var(--m));
		float: left;
		height: 120%;
		shape-outside: repeating-linear-gradient(
			#f1f1f100 0 calc(var(--f) - 3px),
			#191919 0 var(--f)
		);
	}

  html, body {
 
 
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}

@media (max-width: 768px) {


  .divcontainer div {
    width: var(--s);
    height: calc(var(--s) * 1.1547);
    margin-bottom: calc(var(--m) - var(--s) * 0.2885);
    margin-right: 1px;
  }

  .outter {
    width: 180vw; /* increase the width to cover the entire screen */
  }
}


</style>

<script lang="ts" setup>
	import { ref, onBeforeMount } from 'vue';

	const trailIndices = ref<number[]>([]);
	const hoveredColors = [
		'#9B51E0', // Vibrant purple
		'#03DAC6', // Teal/cyan
		'#FF6492', // Soft pink
		'#F2994A', // Orange-yellow
		'#6FCF97', // Green
		'#2F80ED', // Blue
	];

	const hexagonCount = ref(800); // Default value for small devices
  
	onBeforeMount(() => {
		if (window.innerWidth >= 768 && window.innerWidth < 1200) {
			hexagonCount.value = 1200; // Set to 1500 for medium devices
		} else if (window.innerWidth >= 1200) {
			hexagonCount.value = 1700; // Set to 2000 for large devices
		}
	})
  
	const hexagonColors = ref<string[]>(Array(4500).fill('rgb(25, 25, 25)'));

	function handleMouseEnter(index: number) {
		if (!trailIndices.value.includes(index)) {
			trailIndices.value.push(index);
			hexagonColors.value[index] =
				hoveredColors[Math.floor(Math.random() * hoveredColors.length)];
		}

		setTimeout(() => {
			const idx = trailIndices.value.indexOf(index);
			if (idx > -1) {
				trailIndices.value.splice(idx, 1);
				hexagonColors.value[index] = 'rgb(25, 25, 25)'; // fade out
			}
		}, 300);
	}
</script>