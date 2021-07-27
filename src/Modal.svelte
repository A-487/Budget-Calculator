<script>
 import {blur,slide,scale,fade,fly} from 'svelte/transition';
 import {quintOut} from 'svelte/easing';
</script>

<div class="modal-container" in:blur out:fade>
 <div class="modal-content" transition:fly={{y:200}}>
   <slot><!--optional fallback --></slot>
 </div>
</div>