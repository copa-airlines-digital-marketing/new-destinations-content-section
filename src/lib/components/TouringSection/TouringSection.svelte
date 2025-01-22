<script>
	export let image

</script>
<div class="container mx-auto py-8">
    <slot></slot>
      

    <picture class=" block sm:aspect-[21_/_9] pt-6">
    <source media="(min-width: 1367px)" srcset="https://cm-marketing.directus.app/assets/{image}" sizes="">
    <source media="(min-width: 960px)" srcset="https://cm-marketing.directus.app/assets/{image}" sizes="">
    <source media="(min-width: 600px)" srcset="https://cm-marketing.directus.app/assets/{image}" sizes="">
    <img src="https://cm-marketing.directus.app/assets/{image}" alt="" class="w-full h-full object-cover object-bottom rounded-2xl drop-shadow-lg">
</picture>
</div>