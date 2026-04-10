<script lang="ts">
    let isOpen = $state(false)
    function toggle () {
        isOpen = !isOpen
    }
</script>
<section class="gate">
    {#if !isOpen}  
        <button class="gate-btn " onclick={toggle}>
        Gate Dark souls
        </button>
    {/if}
    {#if isOpen}
        <div class="gate-content">
            <p>Welcome to the world of Dark Souls!</p>
            <p>Prepare to die...</p>
        </div>
    {/if}
</section>