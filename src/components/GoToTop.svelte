<script lang="ts">
    /* Icons import */
    import Up from "svelte-bootstrap-icons/lib/ArrowUpShort.svelte";

    export let showOnPx = 150;
    let hidden = true;


    /** @function */
    function goTop() {
        document.body.scrollIntoView();
    }


    /** @function */
    function scrollContainer() {
        return document.documentElement || document.body;
    }


    /** @function */
    function handleOnScroll() {
        if (!scrollContainer()) {
            return;
        }

        if (scrollContainer().scrollTop > showOnPx) {
            hidden = false;
        } else {
            hidden = true;
        }
    }

</script>

<style>
  .back-to-top {
    opacity: 1;
    transition: opacity 0.5s, visibility 0.5s;
    position: fixed;
    z-index: 99;
    right: 40px;
    user-select: none;
    bottom: 40px;
    color: white;
    background-color: #11111b;
    border-radius: 20%;
  }

  .back-to-top.hidden {
    opacity: 0;
    visibility: hidden;
  }
</style>

<svelte:window on:scroll={handleOnScroll}  />

<!-- svelte-ignore a11y-click-events-have-key-events -->
<div class="back-to-top" on:click={goTop} class:hidden><Up height={48} width={48}/></div>