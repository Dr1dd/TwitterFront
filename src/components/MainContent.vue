<template>
    <div class="tweets">
        <div class ="home-header"></div>
    </div>
</template>

<script>
export default {
    name: 'Tweets'
}
</script>

<style lang="scss">
.tweets{
    display: flex;
    width: var(--tweet-content-width-l);
    justify-content: center;
    min-height: 100vh;
    margin-left: calc((100vw - var(--tweet-content-width-l) )/ 2.25);
    background:--base-color;
    border-left: 1px solid #2b3640;
    border-right: 1px solid #2b3640;
    z-index: 1;
    .home-header{
        position: fixed;
        top:0;
        height: 50px;
        width: var(--tweet-content-width-l);
        background: --base-color;
        border-bottom: 1px solid #2b3640;
        z-index: 2;
    }
}

</style>