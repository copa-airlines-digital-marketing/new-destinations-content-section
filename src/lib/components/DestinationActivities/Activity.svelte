<script>
    export let title
    export let description
    export let image
    export let alt
</script>



<div class="grid row-span-2 grid-rows-subgrid border border-gray-300 rounded-2xl overflow-hidden">
    <div class="aspect-w-16 aspect-h-9">
        <img class="object-cover w-full h-full"
            src="https://cm-marketing.directus.app/assets/{image}"
            alt="{alt}" />
    </div>
    <div class="m-8 flex flex-col gap-4">
        <h3 class="font-gilroy font-bold text-u2 text-xl text-primary">{title}</h3>
        <p class=" font-suisse text-grey-600 text-b">{description}</p>
    </div>
</div>




