<template>
    <div id="tmpl">
        <mt-swipe :auto="2000">
        <mt-swipe-item v-for="item in list">
            <img :src="item.img">
        </mt-swipe-item>
   
        </mt-swipe>

       
    </div>
</template>

<script>
    export default{
        data(){
            return {
                list: [
    {
      "url": "http://www.itcast.cn/subject/phoneweb/index.html",
      "img": "http://ofv795nmp.bkt.clouddn.com/vuelogobanner1.jpg"
    },
    {
      "url": "http://www.itcast.cn/subject/phoneweb/index.html",
      "img": "http://ofv795nmp.bkt.clouddn.com/vuelogobanner2-1.jpg"
    }
  ]
            }
            
            
        }
    }
</script>

<style scoped lang="less">
    .mint-swipe-item{
        width: 100%;
        height: 300px;
        background-color: pink;
         img{
            width: 100%;
        } 
    }
    .mint-swipe{
        height: 300px;
    }
    

</style>