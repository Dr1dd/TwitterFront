<template>
  <div class="search">
    <div class="search-content-section">
      <div class="search-bar">
        <div class="search-icon">
          <svg viewBox="0 0 24 24"><g><path d="M21.53 20.47l-3.66-3.66C19.195 15.24 20 13.214 20 11c0-4.97-4.03-9-9-9s-9 4.03-9 9 4.03 9 9 9c2.215 0 4.24-.804 5.808-2.13l3.66 3.66c.147.146.34.22.53.22s.385-.073.53-.22c.295-.293.295-.767.002-1.06zM3.5 11c0-4.135 3.365-7.5 7.5-7.5s7.5 3.365 7.5 7.5-3.365 7.5-7.5 7.5-7.5-3.365-7.5-7.5z"></path></g></svg>
        </div>
        <input type="text">
      </div>
      <div class="trends-tab">

      </div>
      <div class="who-to-follow">

      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Search'
}
</script>

<style lang="scss">
.search{
    display: flex;
    justify-content: flex-start;

    flex-grow: 1;
    position: fixed;
    height: 100vh;
    width: calc((100vw - var(--tweet-content-width-l) )/ 1.8);
    right: 0;
    z-index: 2;
}
.search-content-section{
  width: 290px;
  max-width: 350px;
  margin-left: 20px;
}
.search-bar{
  display: flex;
  flex-direction: row;
  align-items: center;
  position: relative;
  min-width: 290px;
  max-width: 350px;
  height: 42px;
  background-color: rgb(37, 51, 65);
  border-radius: 38px;
  margin-top: 5px;
  margin-bottom: 5px;
  border: 1px solid transparent;
  &:focus-within{
    background-color: var(--base-color);
    border: 1px solid var(--twitter-default);
    .search-icon svg{
      fill: var(--twitter-default);
    }
    
    outline: none;
  }
  .search-icon{
    display: flex;
    height: 18.25px;
    width: 40px;
    padding-left: 5px;
    svg{
      fill: rgb(136, 153, 166);
      height: 100%;
      width: 100%;
    }
  }
  input{
    width: 100%;
    background-color: transparent;
    border: none;
    outline: none;
    font-size: 15px;
    padding: 10px;
    padding-top: 12px;
    color: #fff;
  }
}
.trends-tab{
  height: 270px;
  min-width: 290px;
  max-height: 350px;
  background-color: rgb(25, 39, 52);
  margin: 10px 0;
  border-radius: 16px;
}
.who-to-follow{
  min-height: 15rem;
  background-color: rgb(25, 39, 52);
  border-radius: 16px;
}
</style>