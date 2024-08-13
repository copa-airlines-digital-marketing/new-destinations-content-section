<script>
    export let image
</script>


<!--
<div class="w-full grid grid-rows-[1fr_auto] grid-cols-1 container mx-auto mt-4">
    <picture class=" block col-span-full  sm:aspect-[21_/_9] ">
        <source media="(min-width: 1367px)" srcset="https://cm-marketing.directus.app/assets/{image}?width=2500&format=auto" sizes="">
        <source media="(min-width: 960px)" srcset="https://cm-marketing.directus.app/assets/{image}?width=1367&format=auto" sizes="">
        <source media="(min-width: 600px)" srcset="https://cm-marketing.directus.app/assets/{image}?width=960&format=auto" sizes="">
        <img src="https://cm-marketing.directus.app/assets/{image}?width=1000&height=800&format=auto" alt="" class="w-full h-full object-cover object-bottom rounded-t-2xl drop-shadow-lg">
    </picture>
       
    <div class="row-start-3 bg-primary-dark col-span-full container-grid rounded-b-2xl drop-shadow-lg">
        <div class="col-start-2 m-8">
            <slot></slot>
        </div>
        
    </div>
</div>
-->

<div class="row-start-3 col-span-full container-grid border border-b-[1px]">
    <div class="col-start-2 m-8 ">
        <slot ></slot>
    </div>
</div>

<picture class=" block container mx-auto  sm:aspect-[21_/_8] pt-12 ">
    <source media="(min-width: 1367px)" srcset="https://cm-marketing.directus.app/assets/{image}?width=2500&format=auto" sizes="">
    <source media="(min-width: 960px)" srcset="https://cm-marketing.directus.app/assets/{image}?width=1367&format=auto" sizes="">
    <source media="(min-width: 600px)" srcset="https://cm-marketing.directus.app/assets/{image}?width=960&format=auto" sizes="">
    <img src="https://cm-marketing.directus.app/assets/{image}?width=1000&height=800&format=auto" alt="" class="w-full h-full object-cover object-bottom rounded-2xl drop-shadow-lg">
</picture>
