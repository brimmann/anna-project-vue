<template>
  <div id="pic-div">
    <img src="src/assets/details-post-pic.jpg">
  </div>
  <div style="display: flex; flex-direction: column; width: 80%; margin: 30px auto;">
    <div id="empty-div">
      <div class="full-empty"></div>
      <div class="half-empty"></div>
      <div class="full-empty"></div>
      <div class="half-empty"></div>
      <div class="full-empty"></div>
      <div class="half-empty"></div>
      <div class="full-empty"></div>
      <div class="half-empty"></div>
    </div>
    <div id="buttons-div">
      <button>Ver no mapa</button>
      <button>Adicionar</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "DetailViewPage",
};
</script>

<style scoped>
#pic-div {
  background-image: url("../assets/details-post-pic.jpg");
}

.full-empty {
  height: 3px;
  width: 100%;
  background-color: lightgray;
  margin-bottom: 15px;
}

.half-empty {
  height: 3px;
  width: 60%;
  background-color: lightgray;
  margin-bottom: 15px;
}

#buttons-div {
  margin-top: 60px;
  align-self: end;
}

button {
  background: #ff0066;
  color: white;
  border: 2px solid #ff0066;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  border-radius: 30px;
  padding: 5px 10px;
  font-size: 15px;
  margin-left: 10px;
}
</style>
