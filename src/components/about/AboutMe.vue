<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						"Hello there! I'm Tan, welcome to my corner of the digital world! I'm passionate about video making and board games, and I love engaging in the creative process. As a front end developer, I'm inspired by the new applications being created by more capable developers, and I'm constantly seeking new ways to center a div. Join me on this adventure, and let's head to the promised land together. Feel free to reach out if you share similar interests or just want to chat about video games. My contacts are right below. Thanks for stopping by, and I look forward to connecting with you!",
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/profile.jpeg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
