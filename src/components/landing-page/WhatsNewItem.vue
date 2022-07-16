<template>
  <div id="container-div">
    <div
      id="thumb-div"
      :style="{ backgroundImage: 'url(' + picUrl + ')' }"
    ></div>
    <div>
      <h5>{{ title }}</h5>
      <p>{{ body }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "WhatsNewItem",
  props: ["picUrl", "title", "body"],
};
</script>

<style scoped>
#container-div {
  border: 2px solid #ff0066;
  border-radius: 30px;
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
  padding: 16px 10px;
}
p,
h5 {
  margin-bottom: 8px;
  padding: 0;
}
h5 {
  font-size: 14px;
  color: #e8a0e8;
  margin-top: 0;
}
p {
  font-size: 13px;
}

img {
  min-height: 100%;
}

#thumb-div {
  width: 80px;
  height: 88px;
  flex-shrink: 0;
  overflow: hidden;
  border: 2px solid #ff0066;
  border-radius: 20px;
  margin-right: 10px;
  background-size: cover;
}
</style>
