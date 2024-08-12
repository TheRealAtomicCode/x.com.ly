<script setup lang="ts">
	import { ref } from 'vue';

	const textIndex = ref<0 | 1 | 2 | 3 | 4>(0);

	const letters =
		'ABCDEFGHIJKLMNOPQRSTUVWXYZ 1234567890!.@#$%^&*()_-卡德尔卡迈勒';

	const listOfTitles: string[] = [
		'  X.COM.LY ',
		'QADER BAGHI',
		' X.COM.LY  ',
		' عبدالقادر ',
		'   原子密码    ',
	];

	const name = ref<string>('X.COM.LY   ');

	const changeText = () => {
		let iterations = 1 / 4;

		textIndex.value += 1;
		if (textIndex.value === 5) {
			textIndex.value = 0;
		}

		const interval = setInterval(() => {
			const word = name.value
				.split('')
				.map((letter, index) => {
					if (index < iterations) {
						return listOfTitles[textIndex.value][index];
					}

					return letters[Math.floor(Math.random() * 48)];
				})
				.join('');
			name.value = word;

			if (iterations >= listOfTitles[textIndex.value].length)
				clearInterval(interval);

			iterations += 1;
		}, 40);
	};
</script>

<template>
	<div class="container">
		<h1
			:data-text="name"
			:dir="textIndex !== 3 ? 'ltr' : 'rtl'"
			:class="
				textIndex === 0 || textIndex === 1 || textIndex === 4
					? 'eng'
					: textIndex === 3
					? 'ar'
					: 'bar'
			"
			class="text middle mt top-1/3 left-1/3 text-center flex text-gray-800 font-bold absolute z-20"
		>
			<span @mouseover="changeText">{{ name }}</span
			><span v-if="textIndex !== 2" class="cursor-block"></span>
		</h1>
	</div>
</template>

<style scoped>
	@import url('https://fonts.googleapis.com/css2?family=Cairo:wght@200..1000&family=Jersey+10&family=Jersey+25&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Cairo:wght@200..1000&family=Jersey+10&family=Jersey+25&family=Libre+Barcode+39+Extended+Text&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Cairo:wght@200..1000&family=Jersey+10&family=Jersey+25&family=Libre+Barcode+39+Extended+Text&family=Roboto+Flex:opsz,wght@8..144,100..1000&display=swap');
	.cursor-block {
		display: inline-block;

		background-color: #313131;
		animation: blink 0.7s steps(1, start) infinite;
	}

	@keyframes blink {
		50% {
			opacity: 0;
		}
	}

	.ar {
		font-family: 'Cairo', sans-serif;
		font-optical-sizing: auto;
		font-weight: 700;
	}

	.bar {
		font-family: 'Libre Barcode 39 Extended Text', system-ui;
		font-weight: 400;
		font-style: normal;
	}

	.eng {
		font-family: 'Roboto Flex', sans-serif;
		font-optical-sizing: auto;
	}

	.middle {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);
	}

	.text {
		color: #ffffff;
		text-transform: uppercase;
		font-size: 4rem; /* Adjust the base font size */
	}

	.text::before,
	.text::after {
		content: attr(data-text);
		position: absolute;

		width: 100%;
		height: 100%;
		z-index: -1;
	}

	.text::before {
		color: #ff00c1;
		animation: glitch-effect 3s infinite;
	}

	.text::after {
		color: #3498db;
		animation: glitch-effect 2s infinite;
	}

	@keyframes glitch-effect {
		0% {
			left: -2px;
			top: -2px;
		}
		12% {
			left: 0px;
			top: 2px;
		}
		25% {
			left: 2px;
			top: 0px;
		}
		50% {
			left: -1px;
			top: 3px;
		}
		60% {
			left: 2px;
			top: 1px;
		}
		75% {
			left: -2px;
			top: -1px;
		}
		85% {
			left: 2px;
			top: 1px;
		}
		100% {
			left: 0px;
			top: -2px;
		}
	}

	@media (max-width: 867px) {
		.text {
			font-size: 2rem; /* Adjust the font size for smaller screens */
		}
	}
	@media (min-width: 867px) {
		.text {
			font-size: 5rem; /* Adjust the font size for smaller screens */
		}
	}
</style>