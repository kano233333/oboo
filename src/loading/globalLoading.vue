<template>
  <div class="global_loading" ref="loading"></div>
</template>

<script>
  export default {
    name: "globalLoading",
    data(){
      return {
        count:0
      }
    },
    props:{
      imgs:{
        type:Array,
        default:[]
      }
    },
    mounted(){
      this.preload();
    },
    methods:{
      preload(){
        let _this = this;
        if(this.imgs.length==0){
          this.$refs.loading.style.left = "200%";
          return;
        }
        this.imgs.map(function(item){
          let img = _this.imgPath+item.substring(1,item.length);
          let image = new Image();
          image.src = img;
          image.onload = () => {
            _this.count++;
            _this.$refs.loading.style.left = _this.count/_this.imgs.length*100 +'%';
            if(_this.count == _this.imgs.length){
              _this.$refs.loading.style.left = "200%";
            }
          }
        })
      }
    }
  }
</script>

<style scoped>
</style>