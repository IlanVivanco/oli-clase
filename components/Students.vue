<template>
	<ul class="flex flex-wrap justify-center">
		<li
			v-for="(person, index) in students"
			:key="person.name"
			class="w-2/3 md:w-48 m-4"
		>
			<div
				class="
					rounded-lg
					shadow-md
					bg-white
					hover:shadow-xl
					transition-shadow
					duration-300
					ease-in-out
					p-2
				"
			>
				<div>
					<img
						:src="person.image"
						:alt="person.name"
						class="rounded-md object-cover h-full w-full"
					/>
				</div>

				<div class="px-1">
					<header class="leading-tight my-2">
						<h1
							class="
								text-lg
								font-semibold
								text-blue-900
								flex
								items-center
							"
						>
							<span
								class="
									rounded-full
									bg-gray-200
									text-blue-800
									font-semibold
									px-2
									block
									mr-2
									flex
									justify-center
									items-center
									text-xs
								"
								>{{ index + 1 }}</span
							>
							{{ person.name }}
						</h1>
						<p class="text-gray-500 text-sm">{{ person.age }}</p>
					</header>
				</div>
			</div>
		</li>
	</ul>
</template>

<script>
export default {
	name: "Students",
	data() {
		return {
			students: [
				{
					name: "Le Bebé",
					age: "1 año",
					image: "./images/le-bebe.jpg",
				},
				{
					name: "Lilita",
					age: "3 años",
					image: "./images/lilita.jpg",
				},
				{
					name: "Olivia",
					age: "5 años",
					image: "./images/olivia.jpg",
				},
				{
					name: "Frutillita",
					age: "2 meses",
					image: "./images/frutillita.jpg",
				},
				{
					name: "Abril Kakaka",
					age: "3 años",
					image: "./images/abril.jpg",
				},
				{
					name: "Olafitite",
					age: "3 meses",
					image: "./images/olafitite.jpg",
				},
				{
					name: "Olaf",
					age: "3 años",
					image: "./images/olafite.jpg",
				},
				{
					name: "Olafite",
					age: "4 años",
					image: "./images/olaf.jpg",
				},
				{
					name: "Perri",
					age: "1 año",
					image: "./images/perri.jpg",
				},
				{
					name: "Woody",
					age: "10 años",
					image: "./images/woody.jpg",
				},
				{
					name: "Jessie",
					age: "12 años",
					image: "./images/jessie.jpg",
				},
				{
					name: "Luni",
					age: "4 años",
					image: "./images/luni.jpg",
				},
				{
					name: "Begonia",
					age: "7 años",
					image: "./images/begonia.jpg",
				},
				{
					name: "Clemente",
					age: "1 mes",
					image: "./images/clemente.jpg",
				},
				{
					name: "Ollo",
					age: "2 años",
					image: "./images/ollo.jpg",
				},
				{
					name: "Pellegrini",
					age: "1 año",
					image: "./images/pellegrini.jpg",
				},
				{
					name: "Olivia",
					age: "3 años",
					image: "./images/olivia-coco.jpg",
				},
				{
					name: "Jira",
					age: "3 años",
					image: "./images/pituin.jpg",
				},
				{
					name: "Inca y Lili",
					age: "9 años / 3 meses",
					image: "./images/inca.jpg",
				},
				{
					name: "Cody",
					age: "3 años",
					image: "./images/cody.jpg",
				},
			],
		};
	},
};
</script>
