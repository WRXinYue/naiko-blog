<script setup>
import { onMounted } from 'vue';

const arr = [];

onMounted(() => {
  for (let i = 1; i <= 4; i++) {
    let num = prompt(`${i}`);
    arr.push(num);
  }
  console.log(arr);
  document.write(`<div class="box">`)
    for(let i = 0;i<arr.length;i++){
      document.write(`
      <div style="height: 100px;">
      <span>123</span>
      <h4>FIrst Quarter</h4>
    </div>
      `)
    }
    document.write(`</div>`)
});
</script>

<template>
  <div class="box">
    <div style="height: 100px;">
      <span>123</span>
      <h4>FIrst Quarter</h4>
    </div>
    <div style="height: 100px;">
      <span>123</span>
      <h4>FIrst Quarter</h4>
    </div>
    <div style="height: 100px;">
      <span>123</span>
      <h4>FIrst Quarter</h4>
    </div>
    <div style="height: 100px;">
      <span>123</span>
      <h4>FIrst Quarter</h4>
    </div>
  </div>
</template>
<style scoped>
.box{
  display: flex;
  width: 700px;
  height: 300px;
  border-left: 1px solid red;
  border-bottom: 1px solid yellow;
  margin: 50px auto;
  justify-content: space-around;
  align-items: flex-end;
  text-align: center;
}
.box>div{
  display: flex;
  width: 50px;
  background-color: pink;
  flex-direction: column;
  justify-content: space-between;
}
.box div span{
  margin-top: -22px;
}
.box div h4{
  margin-bottom: -35px;
  width: 70px;
  margin-left: -10px;
}

</style>
