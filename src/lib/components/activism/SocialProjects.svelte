<script>
	import { socialProjects } from '../../data/activism/activismData';
</script>

<div class="flex flex-col">
	<h2
		class="mb-2 rounded-xl bg-gray-800 p-4 text-4xl font-bold text-white md:w-8/12 lg:w-8/12 xl:w-8/12"
	>
		My socially responsible startups
	</h2>
	<div class="mb-20 flex max-w-2xl flex-row flex-wrap">
		{#each socialProjects as project}
			<div class="card image-full m-1 w-80 bg-base-100 shadow-xl">
				<figure><img src={project.img} alt={project.title} /></figure>
				<div class="card-body">
					<h2 class="card-title">{project.title}</h2>
					<p>{project.desc}</p>
				</div>
			</div>
		{/each}
	</div>
</div>
