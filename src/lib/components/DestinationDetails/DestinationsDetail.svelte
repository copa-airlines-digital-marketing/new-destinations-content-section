<script>
    export let detailTitle
    export let detailDescription
    export let detailURLText
    export let detailURL
</script>
<div class="  p-4 grid-cols-subgrid grid grid-rows-[auto_auto_auto] "> 
    <div class="flex xs:flex-col sm:flex-col md:flex-row  gap-2 ">
        <slot></slot>
        <div class="flex flex-col ">
            <h3 class="text-primary font-gilroy text-u1 font-bold ">{detailTitle}</h3>
                <p class="font-suisse font-normal text-grey-600 ">{detailDescription}</p>
                    {#if detailURL} 
                    <a href="{detailURL}" class="text-primary hover:underline font-suisse font-normal">{detailURLText}</a>
                    {/if}
        </div> 
    </div> 
</div>




