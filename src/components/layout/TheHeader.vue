<template>
  <div id="header-div">
    <div id="logo-div">
      <img src="../../assets/logo.png" />
    </div>
    <div id="profile-div">
      <img src="../../assets/img.png" />
    </div>
  </div>
</template>

<script>
export default {
  name: "TheHeader",
};
</script>

<style scoped>

#header-div {
  display: flex;
  justify-content: space-between;
  padding: 0 20px;
  margin-top: 30px;

}

#logo-div {
  width: 150px;
}

#profile-div {
  width: 50px;
}
</style>
