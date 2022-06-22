<script>
	export let title;
	import jackalope from '$lib/assets/img/CreativeMember_jackalope.jpg';
	import elk from '$lib/assets/img/Client_Elk.png';
</script>

<!-- This example requires Tailwind CSS v2.0+ -->
<div class="py-12 bg-white">
	<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
		<div class="lg:text-center">
			<p class="mt-2 text-6xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
				{title}
			</p>
			<p class="mt-4 max-w-2xl text-2xl text-gray-500 lg:mx-auto">
				<slot />
			</p>
		</div>

		<div class="mt-10">
			<dl class="space-y-10 md:space-y-0 md:grid md:grid-cols-2 md:gap-x-8 md:gap-y-10">
				<div class="relative">
					<dt>
						<img src={jackalope} alt="jackalope" />
						<p class="ml-16 text-2xl leading-6 font-medium text-gray-900">Creative Members</p>
					</dt>
					<dd class="mt-2 ml-16 text-base text-gray-500">
						For creative leaders or beginners looking to connect with community based projects and
						give back to the local economy. Be a part of workshops, networking events, and
						mentorship.
					</dd>
					<a type="button" href="/" class="button-primary ml-16"> Get Connected </a>
				</div>

				<div class="relative">
					<dt>
						<img src={elk} alt="elk" />
						<p class="ml-16 text-2xl leading-6 font-medium text-gray-900">Clients</p>
					</dt>
					<dd class="mt-2 ml-16 text-base text-gray-500">
						For individuals or organizations within Lander looking for assistance with creative
						services such as web design, writing, or marketing. Get connected with the creative
						individuals who live right in your own backyard.
					</dd>
					<a type="button" href="/" class="button-primary ml-16"> Get Connected </a>
				</div>
			</dl>
		</div>
	</div>
</div>
