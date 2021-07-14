<template>
	<div class="container mx-auto">
    <h1 class="text-4xl text-blue-900 text-center font-bold mb-8 uppercase uppercase">Clase de Olivia</h1>
		<ul class="flex flex-wrap justify-center">
			<li v-for="person in people" :key="person.name" class="w-48 m-4">
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
							<h1 class="text-lg font-semibold text-blue-900">
								{{ person.name }}
							</h1>
							<p class="text-gray-500 text-sm">
								{{ person.edad }} años
							</p>
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
					edad: 4,
					image: "https://source.unsplash.com/256x256/?black+baby",
				},
				{
					name: "Lilita",
					edad: 3,
					image: "https://source.unsplash.com/256x256/?purple+doll",
				},
				{
					name: "Lola",
					edad: 4,
					image: "https://source.unsplash.com/256x256/?baby,doll",
				},
				{
					name: "Frutillita",
					edad: 4,
					image: "https://source.unsplash.com/256x256/?strawberry",
				},
				{
					name: "Kakaka",
					edad: 3,
					image: "https://source.unsplash.com/256x256/?doll",
				},
				{
					name: "Olafite",
					edad: 4,
					image: "https://source.unsplash.com/256x256/?teddy",
				},
				{
					name: "Olaf",
					edad: 4,
					image: "https://source.unsplash.com/256x256/?little,bear",
				},
				{
					name: "Perri",
					edad: 3,
					image: "https://source.unsplash.com/256x256/?doggy",
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
