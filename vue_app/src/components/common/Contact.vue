<template>
  <div class="container">
    <!--通讯面板-->
    <mt-index-list>
      <div>
        <!--通讯头-->
        <div class="Head">
          <mt-tab-container>
            <mt-tab-container-item>
              <div style=" margin-bottom: 5px;border-bottom:1px solid #ddd;">
                <img src="@/assets/ic_new_friends.png" alt class="Img">
                <span class="subhead">新的朋友</span>
              </div>
              <div>
                <img src="@/assets/ic_group_chat.png" alt class="Img">
                <span class="subhead">群聊</span>
              </div>
              <div>
                <img src="@/assets/ic_tag.png" alt class="Img">
                <span class="subhead">标签</span>
              </div>
              <div>
                <img src="@/assets/ic_common.png" alt class="Img">
                <span class="subhead">公众号</span>
              </div>
            </mt-tab-container-item>
          </mt-tab-container>
        </div>
      </div>
      <div class="column">
        <mt-index-section index="A">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='AAA中国移动'||
          item.title=='AAA牛车'||
          item.title=='AAA造型师'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="B">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='八戒'||
          item.title=='半真半假'||
          item.title=='Bridget'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="C">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='曹操打车'||
          item.title=='朝阳区'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="D" v-show="list.length!==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='大哥'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="E" v-show="list.length==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='二姐'||
          item.title=='二师兄'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="F" v-show="list.length==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='房东'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="G">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='高长宝'||
          item.title=='GHOST'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="H" v-show="list.length==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='好人一生平安'||
          item.title=='合肥通'||
          item.title=='华泰食品'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="J">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='Jackey'||
          item.title=='隽星营业厅'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="K" v-show="list.length==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='考拉'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="L" v-show="list.length!==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='蓝月'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="M" v-show="list.length==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='MR.chane'||
          item.title=='茉莉花'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="P" v-show="list.length!==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='瓶瓶盖盖'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="Q" v-show="list.length==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='清风扶杨柳'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="R" v-show="list.length==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='瑞雪'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="S">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='三辰'||
          item.title=='撒呕血'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
        <mt-index-section index="T" v-show="list.length==24">
          <div v-for="(item,index) of list" :key="index" v-show="item.title=='涛哥'
           ? true : false">
            <img :src="'http://127.0.0.1:3000/'+item.img" alt>
            <span class="subhead" >{{item.title|cn(item.title)}}</span>
          </div>
        </mt-index-section>
      </div>
    </mt-index-list>
  </div>
</template>
<script>
export default {
  data() {
    return { 
      list:[]
    };
  },
  created() {
    this.loadMsg();
  },
  filters:{
    cn:function(value,n="AAA中国移动"){
      if(n=="AAA中国移动"){ 
        return value="AAA中国移动"
      }else if(n=="AAA牛车"){
        return value="AAA牛车"
      }else if(n=="AAA造型师"){
        return value="AAA造型师"
      }else if(n=="八戒"){
        return value="八戒"
      }else if(n=="半真半假"){
        return value="半真半假"
      }else if(n=="Bridget"){
        return value="Bridget"
      }else if(n=="曹操打车"){
        return value="曹操打车"
      }else if(n=="朝阳区"){
        return value="朝阳区"
      }else if(n=="大哥"){
        return value="大哥"
      }else if(n=="二姐"){
        return value="二姐"
      }else if(n=="二师兄"){
        return value="二师兄"
      }else if(n=="房东"){
        return value="房东"
      }else if(n=="高长宝"){
        return value="高长宝"
      }else if(n=="GHOST"){
        return value="GHOST"
      }else if(n=="好人一生平安"){
        return value="好人一生平安"
      }else if(n=="合肥通"){
        return value="合肥通"
      }else if(n=="华泰食品"){
        return value="华泰食品"
      }else if(n=="Jackey"){
        return value="Jackey"
      }else if(n=="隽星营业厅"){
        return value="隽星营业厅"
      }else if(n=="考拉"){
        return value="考拉"
      }else if(n=="蓝月"){
        return value="蓝月"
      }else if(n=="MR.chane"){
        return value="MR.chane"
      }else if(n=="茉莉花"){
        return value="茉莉花"
      }else if(n=="瓶瓶盖盖"){
        return value="瓶瓶盖盖"
      }else if(n=="清风扶杨柳"){
        return value="清风扶杨柳"
      }else if(n=="瑞雪"){
        return value="瑞雪"
      }else if(n=="三辰"){
        return value="三辰"
      }else if(n=="撒呕血"){
        return value="撒呕血"
      }else if(n=="涛哥"){
        return value="涛哥"
      }else{
        return value=""
      }
    }
  },
  methods: {
    // 过滤器
    loadMsg() {
      var url ="http://127.0.0.1:3000/addr";
      // 发送ajax请求
      this.axios.get(url).then(result => {
        this.list = result.data.data;
        console.log(result)
         for (var i = 0; i < this.list.length; i++) {
           this.list[i].id = i;
         }
          console.log(this.list);
      });
    }
  }
};

</script>
<style scoped>
div {
  position: relative;
  cursor: pointer;
}
.container {
  height: 100%;
  background-color: #fff;
  padding-top: 10px;
  padding-left: 3px;
}
img {
  width: 40px;
  height: 40px;
  border-radius: 5px;
}
.subhead {
  position: absolute;
  margin-top: 10px;
  margin-left: 10px;
}
.Img {
  position: relative;
  width: 40px;
  height: 40px;
}
.Head {
  margin-left: 10px;
  background-color: #fff;
}
.Head div + div {
  margin-bottom: 5px;
  border-bottom: 1px solid #ddd;
}
.column div {
  padding-top: 3px;
  padding-left: 5px;
  margin-left: 5px;
  border-bottom: 1px solid #ddd;
}
</style> 
<style>
div.mint-indexlist-nav {
  position: fixed;
}
.mint-indexsection-index {
  background-color: #eee !important;
  height: 36px;
  line-height: 16px;
  cursor: default;
}
</style>