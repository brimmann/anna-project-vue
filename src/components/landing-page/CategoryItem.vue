<template>
<div id="container-div">
  <div id="thumb-div">
    <img :src="picUrl">
  </div>
  <p>{{ title }}</p>
</div>
</template>

<script>
export default {
  name: "CategoryItem",
  props: ['picUrl', 'title']
};
</script>

<style scoped>
#container-div {
  border: 2px solid #FF0066;
  border-radius: 20px;
  width: 85px;
  overflow: hidden;
}
#thumb-div {
  height: 52px;
  flex-shrink: 0;
  overflow: hidden;
}

p {
  font-size: 10px;
  padding-left: 5px;
}
</style>