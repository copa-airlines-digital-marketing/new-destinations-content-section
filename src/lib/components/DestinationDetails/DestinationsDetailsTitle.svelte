<script>
    export let descriptionTitle
</script>

<div class=" flex gap-2 items-center pb-4">
    <slot></slot> 
    <h3 class="text-primary font-gilroy text-u2 font-bold">{descriptionTitle}</h3>
</div>