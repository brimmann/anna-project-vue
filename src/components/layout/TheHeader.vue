<template>
  <div
    id="header-div"
    :class="{ 'fix-header': this.$route.name === 'details' }"
  >
    <div id="logo-div" v-if="this.$route.name !== 'details'">
      <img src="../../assets/logo.png" />
    </div>
    <div id="back-div" @click="$router.push({ name: 'home' })" v-else>
      <img src="../../assets/back-button.png" />
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

.fix-header {
  position: fixed;
  width: 100%;
  box-sizing: border-box;
}

#back-div {
  width: 45px;
  cursor: pointer;
}
</style>
