<script>
    export let title
    export let description
    export let image
    export let alt
</script>



<div class="grid row-span-2 grid-rows-subgrid border border-gray-300 rounded-2xl ">
    <img class="rounded-t-2xl"
            src="https://cm-marketing.directus.app/assets/{image}?width=1419&height=875&format=auto"
            {alt} />

    <div class="m-8 flex flex-col gap-4">
        <h4 class="font-gilroy font-bold text-u2 text-2xl text-primary">{title}</h4>
        <p class=" font-suisse text-grey-600 text-b">{description}</p>
    </div>
</div>



