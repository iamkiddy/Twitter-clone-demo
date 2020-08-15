<template>
  <div class="menu-content">
      <div class="menu-bar">
          <i class="fab fa-twitter"></i>
          <div class="tabs-section">
            <button v-for="tab in tabs" :key="tab.title" class="button-tabs">
              <i :class="`${tab.icon}`"></i>
              <p class="tab-text">{{ tab.title}}</p>
            </button>
            <button class="tweet-btn">Tweet</button>
          </div>
      </div>
  </div>
</template>

<script>
export default {
 name:"Menu",
 data() {
   return{
   tabs:[
     {icon:"fas fa-home",title:"Home",id:"home"},
     {icon:"fas fa-hashtag",title:"Explore",id:"explore"},
     {icon:"fas fa-bell",title:"Notifications",id:"notifications"},
     {icon:"fas fa-envelope",title:"Messages",id:"messages"},
     {icon:"fas fa-bookmark",title:"Bookmarks",id:"bookmarks"},
     {icon:"fas fa-clipboard-list",title:"List",id:"list"},
     {icon:"fas fa-user",title:"Profile",id:"profile"},
     {icon:"fas fa-ellipsis-h",title:"More",id:"more"},
   ]
   }
 }
}
</script>

<style scoped>
i{
  color:#1DA1F2;
  font-size:30px;
}
.menu-content{
  margin-left:60px;
  width: 300px;
  overflow-y: scroll;
}
li{
  list-style: none;
}
.tabs-section{
  margin-top: 20px;
  margin-left: -15px;
}
.button-tabs{
  border:none;
  background: none;
  display:flex;
  padding :15px;
}
.tab-text{
  font-family: "Roboto",sans-serif;
  font-size:20px;
  font-weight: bold;
  margin-left:30px;
  margin-top:5px;
}
.tweet-btn{
    border: 1px solid transparent;
    padding: .375rem .75rem;
    font-size: 1rem;
    line-height: 1.5;
    border-radius: .25rem;
    background: #1DA1F2 !important;
    border-radius: 50px;
    font-family: Poppins;
    font-size: 15px;
    width: 200px;
    height: 50px;
    color: white !important;
    margin-left:20px;
}
</style>