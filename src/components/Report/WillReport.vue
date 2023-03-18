<template>
  <main>
    <div class="showbar">举报平台</div>
    <div class="xianshihang">
      <span class="mingcheng">违法违规行为:</span>
      <input type="text" class="order-input">
    </div>
    <div class="xianshihang">
      <span class="mingcheng">举报标题:</span>
      <input type="text" class="order-input" placeholder="格式：被举报人+违法违规摘要">
    </div>
    <div class="xianshihang">
      <span class="mingcheng">可疑交易的账户名称:</span>
      <input type="text" class="order-input" placeholder="请输入">
    </div>
    <div class="xianshihang" style="height: 170px;">
      <span class="mingcheng">披露/公开信息内容:</span>
      <textarea placeholder="字数为50-200字" class="gs" cols="30" rows="10"></textarea>
    </div>
    <div class="xianshihang" style="height: 170px;">
      <span class="mingcheng">违法事实:</span>
      <textarea placeholder="字数为100-2000字" class="gs" cols="30" rows="10"></textarea>
    </div>
    <div class="xianshihang">
      <span class="mingcheng">证据材料:</span>
      <span class="sub-will">上传文件</span>
    </div>
    <button class="jubao-want" @click="tianxie" style="color: #fff;">提交</button>
  </main>
</template>

<script>
export default {
  emits:['report'],
  methods: {
      tianxie() {
        if(this.$emit('report','Report'))
        console.log('ok');
    }
  }
}
</script>

<style lang="less">
.sub-will{
  margin-top: 5px;display: inline-block;background-color: #dcebf4;
  width: 90px;
  border-radius: 50%;
  height: 30px;
  line-height: 30px;
  transition: 0.5s linear;
  &:hover{
    cursor: pointer;
    background-color: #26f5f5;
  }
}
</style>