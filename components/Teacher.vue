<template>
	<div class="w-1/2 bg-white shadow-md rounded-lg mx-auto mb-6">
		<div
			class="
				card
				border border-gray-100
				bg-indigo-100
				transition-shadow
				shadow-xl
				rounded-lg
				hover:shadow-xl
			"
		>
			<div class="w-full card__media rounded-t-lg overflow-hidden">
				<img
					:src="teacher.background"
					:alt="teacher.name"
					class="h-56 w-full object-cover"
				/>
			</div>
			<div class="card__media--aside"></div>
			<div class="flex items-center p-4">
				<div class="relative flex flex-col items-center w-full">
					<div
						class="h-24 w-24 rounded-full avatar -mt-16 ring-1 ring-white"
					>
						<img
							class="h-24 w-24 md rounded-full relative"
							:src="teacher.image"
							:alt="teacher.name"
						/>
					</div>
					<div class="text-center">
						<span class="text-2xl text-indigo-900 font-bold">
							{{ teacher.name }}
						</span>
						<p class="text-sm text-gray-400">
							{{ teacher.teaser }}
						</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>


<script>
export default {
	name: "Teacher",
	data() {
		return {
			teacher: {
				name: "Olivia Vivanco Haag",
				title: "Profe de yoga",
				age: "4 años",
				teaser: "Enseño yoga para niñes a todos estos pequeñes.",
				image: "./images/oli.jpg",
				background: "https://images.unsplash.com/photo-1506126613408-eca07ce68773?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=731&q=80",
			},
		};
	},
};
</script>
