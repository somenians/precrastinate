<script lang="ts">
	import '$lib/app.css';
	import * as Carousel from '$lib/components/ui/carousel/index.js';
	import * as Card from '$lib/components/ui/card/index.js';
	import { features } from './features';
</script>

<div class="pt-32">
	<Carousel.Root class="w-full max-w-md" opts={{ loop: true }}>
		<Carousel.Content>
			{#each features as feature}
				<Carousel.Item>
					<div class="p-1">
						<Card.Root>
							<Card.Content
								class="flex flex-col aspect-square text-center items-center justify-center p-6"
							>
								<span class="text-2xl font-semibold select-none mb-8">{feature.title}</span>
								<p class="text-xl select-none">{feature.desc}</p>
							</Card.Content>
						</Card.Root>
					</div>
				</Carousel.Item>
			{/each}
		</Carousel.Content>
		<Carousel.Previous />
		<Carousel.Next />
	</Carousel.Root>
</div>
