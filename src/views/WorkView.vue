<template>
	<div class="w-full px-4 text-white bg-[#191919] min-h-[100vh]">
		<div class="max-w-[60rem] mx-auto py-8">
			<h1 class="text-center text-3xl mb-8 mt-9">
				Work Experience and Company Projects
			</h1>
			<div class="bg-gray-800 p-4 rounded-lg mb-6 text-center text-yellow-400">
				Note: The projects mentioned are internal software for Masarat Fintech
				and cannot be shared publicly. Please contact me to view code snippets.
			</div>
			<div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
				<div
					class="max-w-sm border rounded-lg shadow bg-gray-800 border-gray-700 mx-auto"
				>
					<div class="p-5">
						<a href="#">
							<h5
								class="mb-2 text-2xl font-bold tracking-tight text-white"
							>
								Centralized User Management System
							</h5>
						</a>
						<p class="mb-3 font-normal text-gray-400">
							The user management system allows company administrators to manage
							sites, departments, and user accounts. Administrators can create,
							edit, and delete sites, departments, and employees. Each user is
							assigned to a department chich itself has access to different
							internal sites, with granular permission controls at the site
							level. The system exposes an authentication API (ExternalAPI) that
							validates user credentials and returns an access token for use
							across the company's internal systems. This centralized approach
							ensures consistent user access and improved security.
						</p>
						<div class="flex gap-2">
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-teal-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">C#</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-green-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">Vue</span>
							</div>

							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-red-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">ASP.NET Core</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-yellow-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">MSSQL</span>
							</div>
						</div>
					</div>
				</div>

				<div
					class="max-w-sm border rounded-lg shadow bg-gray-800 border-gray-700 mx-auto"
				>
					<div class="p-5">
						<a href="#">
							<h5
								class="mb-2 text-2xl font-bold tracking-tight text-white"
							>
								Customer Tracker
							</h5>
						</a>
						<p class="mb-3 font-normal text-gray-400">
							The customer tracking system allows customer service to manage
							customer accounts, view details, and track interactions.
							Representatives can access customer profiles, purchase history,
							and support tickets in a centralized platform. Managers can
							generate reports to analyze customer activity and representative
							performance. The system integrates with other business systems to
							provide a comprehensive view of customer relationships.
						</p>
						<div class="flex gap-2">
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-teal-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">C#</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-green-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">Vue</span>
							</div>

							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-red-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">ASP.NET Core</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-yellow-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">MSSQL</span>
							</div>
						</div>
					</div>
				</div>

				<div
					class="max-w-sm border rounded-lg shadow bg-gray-800 border-gray-700 mx-auto"
				>
					<div class="p-5">
						<a href="#">
							<h5
								class="mb-2 text-2xl font-bold tracking-tight text-white"
							>
								Transaction Settilement
							</h5>
						</a>
						<p class="mb-3 font-normal text-gray-400">
							The settlement site reconciles payments, transactions, and banking
							services against the company's internal records. Using algorithmic
							optimizations, the site can rapidly process hundreds of thousands
							of records. The system identifies discrepancies and generates
							reports to ensure financial accuracy and compliance. Seamless
							integration with the company's data systems provides a
							comprehensive view of all financial activities.
						</p>
						<div class="flex gap-2">
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-teal-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">C#</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-green-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">Vue</span>
							</div>

							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-red-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">ASP.NET Core</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-yellow-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">MSSQL</span>
							</div>
						</div>
					</div>
				</div>

				<!-- Add more project cards as needed -->
			</div>

			<h1 class="text-center text-3xl mb-8 mt-9">Personal Projects</h1>

			<div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
				<div
					class="max-w-sm border rounded-lg shadow bg-gray-800 border-gray-700 mx-auto"
				>
					<div class="p-5">
						<a
							href="https://github.com/TheRealAtomicCode/Depricated-DeviseHR-Server"
						>
							<h5
								class="mb-2 text-2xl font-bold tracking-tight text-white"
							>
								DeviseHR (work in progress)
							</h5>
						</a>
						<p class="mb-3 font-normal text-gray-400">
							The Backend for my (maybe startup... idk) SaaS project DeviseHR,
							its a HR system designed to manage employees, calculate leave, and
							manage clockins for verious companies. Note: this is an older
							version of the code, i created a newer repo, and made this public
							because I later didn't like the database design and changed a few
							things, contact me to view a better version of the code.
						</p>
						<div class="flex gap-2">
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-teal-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">C#</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-blue-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">PostgreSQL</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-red-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">ASP.NET Core</span>
							</div>
						</div>

						<div class="flex gap-2 mt-4">
							<a
								href="https://github.com/TheRealAtomicCode/Depricated-DeviseHR-Server"
								class="inline-flex items-center rounded-lg bg-blue-700 py-2 px-3 text-center text-sm font-medium text-white hover:bg-blue-800 focus:outline-none focus:ring-4 focus:ring-blue-300 bg-blue-600 hover:bg-blue-700 focus:ring-blue-800"
							>
								<svg
									aria-hidden="true"
									class="mr-2 -ml-1 h-5 w-5"
									fill="currentColor"
									viewBox="0 0 20 20"
									xmlns="http://www.w3.org/2000/svg"
								>
									<path
										d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"
									/>
								</svg>
								View on GitHub
							</a>
						</div>
					</div>
				</div>

				<div
					class="max-w-sm border rounded-lg shadow bg-gray-800 border-gray-700 mx-auto"
				>
					<div class="p-5">
						<a href="https://github.com/TheRealAtomicCode/chat-express-2020">
							<h5
								class="mb-2 text-2xl font-bold tracking-tight text-white"
							>
								Chat App
							</h5>
							<h4>Initial wait due to server sleep (free tier)</h4>
						</a>
						<p class="mb-3 font-normal text-gray-400">
							An MVC Chat app written in Node.JS i wrote when learning web
							sockets
						</p>
						<div class="flex gap-2">
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-blue-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">Node.JS</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-teal-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">CSS</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-red-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">Express</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-yellow-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">Socket.IO</span>
							</div>
						</div>

						<div class="mt-4 flex gap-2">
							<a
								href="https://github.com/TheRealAtomicCode/chat-express-2020"
								class="inline-flex items-center rounded-lg bg-blue-700 py-2 px-3 text-center text-sm font-medium text-white hover:bg-blue-800 focus:outline-none focus:ring-4 focus:ring-blue-300 bg-blue-600 hover:bg-blue-700 focus:ring-blue-800"
							>
								<svg
									aria-hidden="true"
									class="mr-2 -ml-1 h-5 w-5"
									fill="currentColor"
									viewBox="0 0 20 20"
									xmlns="http://www.w3.org/2000/svg"
								>
									<path
										d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"
									/>
								</svg>
								View on GitHub
							</a>
							<a
								href="https://chat-express-2020.onrender.com"
								class="inline-flex items-center rounded-lg bg-green-700 py-2 px-3 text-center text-sm font-medium text-white hover:bg-green-800 focus:outline-none focus:ring-4 focus:ring-green-300 bg-green-600 hover:bg-green-700 focus:ring-green-800"
							>
								<svg
									aria-hidden="true"
									class="mr-2 -ml-1 h-5 w-5"
									fill="currentColor"
									viewBox="0 0 20 20"
									xmlns="http://www.w3.org/2000/svg"
								>
									<path d="M10 12a2 2 0 1 0 0-4 2 2 0 0 0 0 4z" />
									<path
										fill-rule="evenodd"
										d="M.458 10C1.732 5.943 5.522 3 10 3s8.268 2.943 9.542 7c-1.274 4.057-5.064 7-9.542 7S1.732 14.057.458 10zM14 10a4 4 0 1 1-8 0 4 4 0 0 1 8 0z"
										clip-rule="evenodd"
									/>
								</svg>
								Visit Website
							</a>
						</div>
					</div>
				</div>

				<div
					class="max-w-sm border rounded-lg shadow bg-gray-800 border-gray-700 mx-auto"
				>
					<div class="p-5">
						<a
							href="https://github.com/TheRealAtomicCode/React-basics---memory-game---Game-of-Thrones"
						>
							<h5
								class="mb-2 text-2xl font-bold tracking-tight text-white"
							>
								Simple Memory game
							</h5>
						</a>
						<p class="mb-3 font-normal text-gray-400">
							A simple memory game I build when learning react hooks, buck when
							hooks were kinda new, and used react
						</p>
						<div class="flex gap-2">
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-blue-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">React</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-teal-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">CSS</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-red-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">Hooks</span>
							</div>
						</div>

						<div class="mt-4 flex gap-2">
							<a
								href="https://github.com/TheRealAtomicCode/React-basics---memory-game---Game-of-Thrones"
								class="inline-flex items-center rounded-lg bg-blue-700 py-2 px-3 text-center text-sm font-medium text-white hover:bg-blue-800 focus:outline-none focus:ring-4 focus:ring-blue-300 bg-blue-600 hover:bg-blue-700 focus:ring-blue-800"
							>
								<svg
									aria-hidden="true"
									class="mr-2 -ml-1 h-5 w-5"
									fill="currentColor"
									viewBox="0 0 20 20"
									xmlns="http://www.w3.org/2000/svg"
								>
									<path
										d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"
									/>
								</svg>
								View on GitHub
							</a>
							<a
								href="https://66ba5eee5624611b61af0432--boisterous-maamoul-30481e.netlify.app/"
								class="inline-flex items-center rounded-lg bg-green-700 py-2 px-3 text-center text-sm font-medium text-white hover:bg-green-800 focus:outline-none focus:ring-4 focus:ring-green-300 bg-green-600 hover:bg-green-700 focus:ring-green-800"
							>
								<svg
									aria-hidden="true"
									class="mr-2 -ml-1 h-5 w-5"
									fill="currentColor"
									viewBox="0 0 20 20"
									xmlns="http://www.w3.org/2000/svg"
								>
									<path d="M10 12a2 2 0 1 0 0-4 2 2 0 0 0 0 4z" />
									<path
										fill-rule="evenodd"
										d="M.458 10C1.732 5.943 5.522 3 10 3s8.268 2.943 9.542 7c-1.274 4.057-5.064 7-9.542 7S1.732 14.057.458 10zM14 10a4 4 0 1 1-8 0 4 4 0 0 1 8 0z"
										clip-rule="evenodd"
									/>
								</svg>
								Visit Website
							</a>
						</div>
					</div>
				</div>

				<div
					class="max-w-sm border rounded-lg shadow bg-gray-800 border-gray-700 mx-auto"
				>
					<div class="p-5">
						<a href="https://github.com/AQbaghi/task-manager-api-nodecourse">
							<h5
								class="mb-2 text-2xl font-bold tracking-tight text-white"
							>
								Task Manager API
							</h5>
						</a>
						<p class="mb-3 font-normal text-gray-400">
							A REST API built in Express and Mongoose, I built out of curiosity
							to find out what NoSQL is about, ehh... MySQL is better for most
							projects (most not all).
						</p>
						<div class="flex gap-2">
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-green-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">Node.JS</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-red-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">Express</span>
							</div>
							<div
								class="relative grid select-none items-center whitespace-nowrap rounded-lg bg-blue-500 py-1.5 px-3 font-sans text-xs font-bold uppercase text-white"
							>
								<span class="">MongoDB</span>
							</div>
						</div>

						<div class="mt-4 flex gap-2">
							<a
								href="https://github.com/AQbaghi/task-manager-api-nodecourse"
								class="inline-flex items-center rounded-lg bg-blue-700 py-2 px-3 text-center text-sm font-medium text-white hover:bg-blue-800 focus:outline-none focus:ring-4 focus:ring-blue-300 bg-blue-600 hover:bg-blue-700 focus:ring-blue-800"
							>
								<svg
									aria-hidden="true"
									class="mr-2 -ml-1 h-5 w-5"
									fill="currentColor"
									viewBox="0 0 20 20"
									xmlns="http://www.w3.org/2000/svg"
								>
									<path
										d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"
									/>
								</svg>
								View on GitHub
							</a>
						</div>
					</div>
				</div>

				<!-- Add more project cards as needed -->
			</div>
		</div>
	</div>
</template>

<script setup lang="ts"></script>

<style></style>
