<script>
    export let image
</script>

<div class="w-full grid grid-rows-[1fr_auto] grid-cols-1">
    <picture class=" block col-span-full  sm:aspect-[21_/_9] ">
        <source media="(min-width: 1367px)" srcset="https://cm-marketing.directus.app/assets/{image}}?width=2500&format=auto" sizes="">
        <source media="(min-width: 960px)" srcset="https://cm-marketing.directus.app/assets/{image}}?width=1367&format=auto" sizes="">
        <source media="(min-width: 600px)" srcset="https://cm-marketing.directus.app/assets/{image}}?width=960&format=auto" sizes="">
        <img src="https://cm-marketing.directus.app/assets/{image}}?width=1000&height=800&format=auto" alt="" class="w-full h-full object-cover object-bottom ">
    </picture>
       
    <div class="row-start-3 py-8 bg-backgound-paper col-span-full container-grid">
        <div class=" col-start-2">
            <slot></slot>
        </div>
        
    </div>
</div>
