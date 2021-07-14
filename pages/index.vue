<template>
	<div class="container mx-auto">
		<h1
			class="
				text-4xl text-blue-900 text-center
				font-bold
				mb-8
				uppercase uppercase
			"
		>
			Clase de Olivia
		</h1>
		<ul class="flex flex-wrap justify-center">
			<li
				v-for="(person, index) in people"
				:key="person.name"
				class="w-48 m-4"
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
							<h1 class="text-lg font-semibold text-blue-900 flex items-center">
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
							<p class="text-gray-500 text-sm">{{ person.edad }}</p>
						</header>
					</div>
				</div>
			</li>
		</ul>
	</div>
</template>

<script>
export default {
	layout: "default",
	name: "Home",
	data() {
		return {
			people: [
				{
					name: "Le Bebé",
					edad: "1 año",
					image: "https://source.unsplash.com/256x256/?black+baby",
				},
				{
					name: "Lilita",
					edad: "3 años",
					image: "https://source.unsplash.com/256x256/?purple+doll",
				},
				{
					name: "Olivia",
					edad: "5 años",
					image: "https://source.unsplash.com/256x256/?baby+doll",
				},
				{
					name: "Frutillita",
					edad: "2 meses",
					image: "https://source.unsplash.com/256x256/?strawberry",
				},
				{
					name: "Abril",
					edad: "3 años",
					image: "https://source.unsplash.com/256x256/?doll",
				},
				{
					name: "Olafitite",
					edad: "3 meses",
					image: "https://source.unsplash.com/256x256/?teddy+purple",
				},
				{
					name: "Olafite",
					edad: "3 años",
					image: "https://source.unsplash.com/256x256/?teddy",
				},
				{
					name: "Olaf",
					edad: "5 años",
					image: "https://source.unsplash.com/256x256/?little,bear",
				},
				{
					name: "Perri",
					edad: "1 año",
					image: "https://source.unsplash.com/256x256/?doggy",
				},
				{
					name: "Woody",
					edad: "10 años",
					image: "https://source.unsplash.com/256x256/?woody",
				},
				{
					name: "Jessie",
					edad: "12 años",
					image: "https://source.unsplash.com/256x256/?jessie",
				},
				{
					name: "Luni",
					edad: "8 años",
					image: "https://source.unsplash.com/256x256/?unicorn",
				},
				{
					name: "Begonia",
					edad: "7 años",
					image: "https://source.unsplash.com/256x256/?doll+cloth",
				},
				{
					name: "Clemente",
					edad: "1 mes",
					image: "https://source.unsplash.com/256x256/?doll+stripes",
				},
				{
					name: "Tumpú",
					edad: "2 años",
					image: "https://source.unsplash.com/256x256/?elephant",
				},
				{
					name: "Pellegrini",
					edad: "1 años",
					image: "https://source.unsplash.com/256x256/?teddy+bear+white",
				},
				{
					name: "Olivia",
					edad: "3 años",
					image: "https://source.unsplash.com/256x256/?crocodile",
				},
				{
					name: "Pituín",
					edad: "3 años",
					image: "https://source.unsplash.com/256x256/?crocodile",
				},
			],
		};
	},
};
</script>

<style>
.hide-scroll-bar {
	-ms-overflow-style: none;
	scrollbar-width: none;
}
.hide-scroll-bar::-webkit-scrollbar {
	display: none;
}
</style>
