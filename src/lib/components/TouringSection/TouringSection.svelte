<script>
	export let image

</script>
<div class="container mx-auto py-8">
    <slot></slot>
      

    <picture class=" block sm:aspect-[21_/_9] pt-6">
    <source media="(min-width: 1367px)" srcset="https://cm-marketing.directus.app/assets/{image}?width=2500&format=auto&access_token=2NYgIiKkCP6FNY4Jj31_h4d5VKkSSVbZ" sizes="">
    <source media="(min-width: 960px)" srcset="https://cm-marketing.directus.app/assets/{image}?width=1367&format=auto&access_token=2NYgIiKkCP6FNY4Jj31_h4d5VKkSSVbZ" sizes="">
    <source media="(min-width: 600px)" srcset="https://cm-marketing.directus.app/assets/{image}?width=960&format=auto&access_token=2NYgIiKkCP6FNY4Jj31_h4d5VKkSSVbZ" sizes="">
    <img src="https://cm-marketing.directus.app/assets/{image}?width=1000&height=800&format=auto&access_token=2NYgIiKkCP6FNY4Jj31_h4d5VKkSSVbZ" alt="" class="w-full h-full object-cover object-bottom rounded-2xl drop-shadow-lg">
</picture>
</div>