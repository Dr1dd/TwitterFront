<template>
    <div class="tweets">
        <div class ="home-header">
            <div class="header-content">
                  <div class="header-text"> Home</div>
                  <div class="preferences">
                    <svg viewBox="0 0 24 24" ><g><path d="M22.772 10.506l-5.618-2.192-2.16-6.5c-.102-.307-.39-.514-.712-.514s-.61.207-.712.513l-2.16 6.5-5.62 2.192c-.287.112-.477.39-.477.7s.19.585.478.698l5.62 2.192 2.16 6.5c.102.306.39.513.712.513s.61-.207.712-.513l2.16-6.5 5.62-2.192c.287-.112.477-.39.477-.7s-.19-.585-.478-.697zm-6.49 2.32c-.208.08-.37.25-.44.46l-1.56 4.695-1.56-4.693c-.07-.21-.23-.38-.438-.462l-4.155-1.62 4.154-1.622c.208-.08.37-.25.44-.462l1.56-4.693 1.56 4.694c.07.212.23.382.438.463l4.155 1.62-4.155 1.622zM6.663 3.812h-1.88V2.05c0-.414-.337-.75-.75-.75s-.75.336-.75.75v1.762H1.5c-.414 0-.75.336-.75.75s.336.75.75.75h1.782v1.762c0 .414.336.75.75.75s.75-.336.75-.75V5.312h1.88c.415 0 .75-.336.75-.75s-.335-.75-.75-.75zm2.535 15.622h-1.1v-1.016c0-.414-.335-.75-.75-.75s-.75.336-.75.75v1.016H5.57c-.414 0-.75.336-.75.75s.336.75.75.75H6.6v1.016c0 .414.335.75.75.75s.75-.336.75-.75v-1.016h1.098c.414 0 .75-.336.75-.75s-.336-.75-.75-.75z"></path></g></svg>
                  </div>
            </div>
        </div>
        <div class="tweet" v-for="tweet in tweetArray" :key="tweet.id">
            <div class="profile-pic"> <img :src="tweet.profilePic"></div>
            <div class="tweet-content-wrapper">
                <div class="profile-name-wrapper"> 
                    <div class="profile-info">
                        <span class="profile-name">{{tweet.name}}</span>
                        <span class="profile-username">{{tweet.username}}</span> 
                    </div>
                </div>
                <div class="tweet-text"> {{tweet.text}} {{tweet.media}}</div>
                <div v-if="tweet.media != ''" class="tweet-media"> <img :src="tweet.media" alt=""></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Tweets',
    data(){
        return{
            tweetArray: [],
        }
    },
    created: function() {
        this.tweetArray = [{id: 1, name: "John", username: "@johnson", text: "Hello World", media: require('../assets/tweet-images/elephant.jpg'), profilePic: require('../assets/egg.jpg') },
        {id: 2, name: "John", username: "@johnson", text: "Hello World", media: require('../assets/tweet-images/elephant.jpg'), profilePic: require('../assets/egg.jpg')},
        {id: 3, name: "John", username: "@johnson", text: "Hello d", media: "", profilePic: require('../assets/egg.jpg')},
        {id: 4, name: "John", username: "@johnson", text: "Hello d", media: "", profilePic: ""},
        {id: 5, name: "John", username: "@johnson", text: "Hello a", media: "", profilePic: ""},
        {id: 6, name: "John", username: "@johnson", text: "Hello Wsorld", media: "", profilePic: ""},
        ];
    },
}
</script>

<style lang="scss">
$icon-hover-bg-color: rgba(29, 161, 242, 0.1);
$twitter-default: rgba(29, 161, 242, 1.00);
$default-border: 1px solid #2b3640;
.tweets{
    display: flex;
    flex-direction: column;
    width: var(--tweet-content-width-l);
    margin-left: calc((100vw - var(--tweet-content-width-l) )/ 2.25);
    background: var(--base-color);
    border-left: 1px solid #2b3640;
    border-right: 1px solid #2b3640;
    z-index: 1;
    .home-header{
        display: flex;
        position: fixed;
        top:0;
        height: 50px;
        width: var(--tweet-content-width-l);
        background-color: var(--base-color);
        border-bottom: 1px solid #2b3640;
        z-index: 2;
        .header-text{
            color: #fff;
            font-weight: 900;
            cursor: pointer;
        }
        .header-content{
            display: flex;
            flex-direction: row;
            justify-content: space-between;
            align-items: center;
            width: 100%;
            padding-left: 15px;
            padding-right: 5px;
            .preferences{
                display: flex;
                align-items: center;
                justify-content: center;
                height: 40px;
                width: 40px;
                border-radius: 50%;
                transition: background-color 0.25s;
                svg{
                    height: 24px;
                    width: 24px;
                    fill: $twitter-default;
                }
                &:hover{
                    background-color: $icon-hover-bg-color;
                }
            }   
        }
    }
    .tweet{
        display: flex;
        flex-direction: row;
        max-width: 100%;
        min-height: 90px;
        max-height: 520px;
        padding: 10px 15px;
        border-bottom: $default-border;
        color: #fff;
        .profile-pic{
            min-height: 100%;
            padding-right: 10px;
            img{
                height: 49px;
                width: 49px;
                border-radius: 50%;
            }
        }
        .tweet-content-wrapper{
            display: flex;
            flex-direction: column;
            .profile-name-wrapper{
                display: flex;
                flex-direction: row;
                width: 100%;
                justify-content: space-between;
                .profile-info{
                    span{
                        margin-right: 5px;
                        font-size: 15px;
                        font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Ubuntu, "Helvetica Neue", sans-serif;
                    }
                    .profile-name{
                        
                        font-weight: 700;
                    }
                    .profile-username{
                        color: #8899A6;
                    }
                }
            }
            .tweet-text{
                text-align: left;
                font-size: 15px;
                font-weight: 400;
                font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Ubuntu, "Helvetica Neue", sans-serif;
            }
            .tweet-media{
                max-width: 100%;
                max-height: 285px;
                overflow: hidden;
                border-radius: 15px;
                margin-top: 10px;
                img{
                    max-height: 509px;
                    width: 100%;
                    border: $default-border;
                }
            }
        }
    }
}

</style>