<template>
  <div class="search">

  </div>
</template>

<script>
export default {
    name: 'Search'
}
</script>

<style>
.search{
    display: flex;
    justify-content: flex-start;
    flex-grow: 1;
    position: fixed;
    height: 100vh;
    width: calc((100vw - var(--tweet-content-width-l) )/ 1.75);
    right: 0;
    background:--base-color;
    z-index: 2;
}

</style>