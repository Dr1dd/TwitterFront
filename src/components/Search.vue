<template>
  <div class="search">
    <div class="search-content-section">
      <div class="search-bar">
        <div class="search-icon">
          <svg viewBox="0 0 24 24"><g><path d="M21.53 20.47l-3.66-3.66C19.195 15.24 20 13.214 20 11c0-4.97-4.03-9-9-9s-9 4.03-9 9 4.03 9 9 9c2.215 0 4.24-.804 5.808-2.13l3.66 3.66c.147.146.34.22.53.22s.385-.073.53-.22c.295-.293.295-.767.002-1.06zM3.5 11c0-4.135 3.365-7.5 7.5-7.5s7.5 3.365 7.5 7.5-3.365 7.5-7.5 7.5-7.5-3.365-7.5-7.5z"></path></g></svg>
        </div>
        <input type="text" placeholder="Search Twitter">
      </div>
      <div class="trends-tab">
        <div class="trends-header">
          Trends for you
          <div class="trends-settings">
            <svg viewBox="0 0 24 24"><g><path d="M12 8.21c-2.09 0-3.79 1.7-3.79 3.79s1.7 3.79 3.79 3.79 3.79-1.7 3.79-3.79-1.7-3.79-3.79-3.79zm0 6.08c-1.262 0-2.29-1.026-2.29-2.29S10.74 9.71 12 9.71s2.29 1.026 2.29 2.29-1.028 2.29-2.29 2.29z"></path><path d="M12.36 22.375h-.722c-1.183 0-2.154-.888-2.262-2.064l-.014-.147c-.025-.287-.207-.533-.472-.644-.286-.12-.582-.065-.798.115l-.116.097c-.868.725-2.253.663-3.06-.14l-.51-.51c-.836-.84-.896-2.154-.14-3.06l.098-.118c.186-.222.23-.523.122-.787-.11-.272-.358-.454-.646-.48l-.15-.014c-1.18-.107-2.067-1.08-2.067-2.262v-.722c0-1.183.888-2.154 2.064-2.262l.156-.014c.285-.025.53-.207.642-.473.11-.27.065-.573-.12-.795l-.094-.116c-.757-.908-.698-2.223.137-3.06l.512-.512c.804-.804 2.188-.865 3.06-.14l.116.098c.218.184.528.23.79.122.27-.112.452-.358.477-.643l.014-.153c.107-1.18 1.08-2.066 2.262-2.066h.722c1.183 0 2.154.888 2.262 2.064l.014.156c.025.285.206.53.472.64.277.117.58.062.794-.117l.12-.102c.867-.723 2.254-.662 3.06.14l.51.512c.836.838.896 2.153.14 3.06l-.1.118c-.188.22-.234.522-.123.788.112.27.36.45.646.478l.152.014c1.18.107 2.067 1.08 2.067 2.262v.723c0 1.183-.888 2.154-2.064 2.262l-.155.014c-.284.024-.53.205-.64.47-.113.272-.067.574.117.795l.1.12c.756.905.696 2.22-.14 3.06l-.51.51c-.807.804-2.19.864-3.06.14l-.115-.096c-.217-.183-.53-.23-.79-.122-.273.114-.455.36-.48.646l-.014.15c-.107 1.173-1.08 2.06-2.262 2.06zm-3.773-4.42c.3 0 .593.06.87.175.79.328 1.324 1.054 1.4 1.896l.014.147c.037.4.367.7.77.7h.722c.4 0 .73-.3.768-.7l.014-.148c.076-.842.61-1.567 1.392-1.892.793-.33 1.696-.182 2.333.35l.113.094c.178.148.366.18.493.18.206 0 .4-.08.546-.227l.51-.51c.284-.284.305-.73.048-1.038l-.1-.12c-.542-.65-.677-1.54-.352-2.323.326-.79 1.052-1.32 1.894-1.397l.155-.014c.397-.037.7-.367.7-.77v-.722c0-.4-.303-.73-.702-.768l-.152-.014c-.846-.078-1.57-.61-1.895-1.393-.326-.788-.19-1.678.353-2.327l.1-.118c.257-.31.236-.756-.048-1.04l-.51-.51c-.146-.147-.34-.227-.546-.227-.127 0-.315.032-.492.18l-.12.1c-.634.528-1.55.67-2.322.354-.788-.327-1.32-1.052-1.397-1.896l-.014-.155c-.035-.397-.365-.7-.767-.7h-.723c-.4 0-.73.303-.768.702l-.014.152c-.076.843-.608 1.568-1.39 1.893-.787.326-1.693.183-2.33-.35l-.118-.096c-.18-.15-.368-.18-.495-.18-.206 0-.4.08-.546.226l-.512.51c-.282.284-.303.73-.046 1.038l.1.118c.54.653.677 1.544.352 2.325-.327.788-1.052 1.32-1.895 1.397l-.156.014c-.397.037-.7.367-.7.77v.722c0 .4.303.73.702.768l.15.014c.848.078 1.573.612 1.897 1.396.325.786.19 1.675-.353 2.325l-.096.115c-.26.31-.238.756.046 1.04l.51.51c.146.147.34.227.546.227.127 0 .315-.03.492-.18l.116-.096c.406-.336.923-.524 1.453-.524z"></path></g></svg>
          </div>
        </div>
      </div>
      <div class="who-to-follow">
        <div class="who-to-folow-header">
          Who to follow
        </div>
        <div class="who-to-follow-content">
          <div class="who-to-follow-user">
            <div class="user-image">
              <img src="../assets/egg.jpg" alt="">
            </div>
            <div class="follow-user-wrapper">
                <div class="follow-user-name">
                  <a href="" class="link-to-user">
                    <div class="user-name"> Egg</div>
                    <div class="user-twitter-name"> @Egginson</div>
                  </a>
                </div>
                <div class="follow-user-btn">
                  Follow
                </div>
            </div>
          </div>
        </div>
        <div class="show-more-users">
              <div class="show-more-btn">Show more</div>
        </div>
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
$box-default-bg-color: rgb(25, 39, 52);
$icon-hover-bg-color: rgba(29, 161, 242, 0.1);
$default-border: 1px solid #2b3640;
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
    &::placeholder{
     color: rgb(136, 153, 166);
     font-weight: 100;
    }
  }
}
.trends-tab{
  height: 270px;
  min-width: 290px;
  max-height: 350px;
  background-color: $box-default-bg-color;
  margin: 10px 0;
  border-radius: 16px;
}

.trends-tab{
  display: flex;
  flex-direction: column;
  .trends-header{
    display: flex;
    justify-content: space-between;
    flex-direction: row;
    padding: 10px;
    padding-left: 15px;
    font-size: 19px;
    color: #fff;
    align-items: center;
    font-weight: 900;
    border-bottom: $default-border;
    .trends-settings{
      display: flex;
      svg{
        fill: var(--twitter-default);
        height: 24px;
        width: 24px;
      }
    }
  }
}
 .who-to-follow{
    background-color: $box-default-bg-color;
    border-radius: 16px;
    .who-to-folow-header{
      display: flex;
      flex-direction: row;
      justify-content: flex-start;
      padding:10px;
      padding-left: 15px;
      font-size: 19px;
      color: #fff;
      font-weight: 900;
      border-bottom: $default-border;
    }
    .who-to-follow-content{
      display: flex;
      flex-direction: column;
      padding:15px;
      border-bottom: $default-border;
      &:hover{
        background-color: rgb(37, 51, 65);
      }
      .who-to-follow-user{
        display: flex;
        align-content: center;
         max-height: 59px;
        .user-image{
          border-radius: 50%;
          max-width: 60px;
          img{
            height: 49px;
            width: 49px;
            border-radius: 50%;
            transition: filter 0.25s;
            cursor: pointer;
            &:hover{
              filter: brightness(0.9);
            }
          }
        }
        .follow-user-wrapper{
          display: flex;
          flex-direction: row;
          width: 100%;
          justify-content: space-between;
          align-self: center;
          margin-left: 10px;
          .follow-user-name{
            a{
              color: #fff;
              text-decoration: none;
              font-size: 15px;
              font-weight: 900;
              cursor: pointer;
              div:nth-child(1):hover{
                text-decoration: underline;
              }
              div:nth-child(2){
                font-weight: 300;
                color: #8899A6;
              }
            }
            .link-to-user{
             text-align: left;
            }
          }
          .follow-user-btn{
            align-self: center;
            border: 1px solid var(--twitter-default);
            border-radius: 30px;
            font-size: 15px;
            font-weight: 900;
            padding: 4px 15px;
            cursor: pointer;
            color: var(--twitter-default);
            transition: background-color 0.25s;
            &:hover{
              background-color: $icon-hover-bg-color;
            }
          }
        }
      }
    }
    .show-more-users{
      display: flex;
      flex-direction: column;
      justify-content: center;
      max-height: 40px;
      width: 100%;
      padding: 15px;
      text-align: center;
      cursor:pointer;
      div{
        text-align: left;
        color: var(--twitter-default);
        font-size: 15px;
      }
    }
  }
</style>