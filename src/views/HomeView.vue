<script setup lang="ts">
	import Background from '../components/Background.vue';
	import HeaderComp from '../components/HeaderComp.vue';
</script>

<template>
	<div>
		<Background />

		<HeaderComp />

		<div class="profile-card">
			<img
				src="../assets/portraid.jpg"
				alt="Portrait"
				class="profile-image grayscale"
			/>
			<div class="text-content">
				<h2 class="name">Fullstack Developer</h2>

				<p class="description">
					Passionate software developer with 2+ years building robust, scalable,
					and user-friendly web applications. Proficient in diverse web
					technologies. Adaptable to the customers requirements with 3+ years of
					service desk experience.
				</p>
			</div>
		</div>
	</div>
</template>

<style>
	.h-screen {
		height: 100vh;
	}

	.rounded-lg {
		border-radius: 0.5rem;
	}

	.shadow-lg {
		box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1),
			0 4px 6px -2px rgba(0, 0, 0, 0.05);
	}

	.object-cover {
		object-fit: cover;
	}

	.profile-card {
		display: flex;
		flex-direction: column;
		align-items: center;
		position: absolute;
		max-width: 42rem;
		margin-top: 110vh;
		left: 50%;
		transform: translateX(-50%);
	}

	.profile-image {
		width: 90%;
		max-width: 26rem;
		height: 22rem;
		object-fit: cover;
		margin-right: 4rem;
		border-radius: 2rem;
	}

	.text-content {
		text-align: center;
		color: white;
		margin-top: 2rem;
	}

	.name {
		font-size: 2rem;
		font-weight: bold;
		margin-bottom: 0.5rem;
	}

	.role {
		color: #e5e7eb; /* Tailwind's gray-200 */
	}

	.description {
		margin-top: 1rem;
		color: #d1d5db; /* Tailwind's gray-300 */
	}

	@media (min-width: 968px) {
		.profile-card {
			width: 42rem;
		}
	}

	@media (min-width: 968px) {
		.profile-card {
			flex-direction: row;
			align-items: flex-start;
			text-align: left;
		}
	}

	@media (min-width: 1024px) {
		.profile-card {
			flex-direction: row;
			align-items: flex-start;
			text-align: left;
			max-width: 100%;
		}

		.profile-image {
			max-width: 18rem;
		}
	}

	.grayscale {
		filter: grayscale(70%);
	}
</style>
