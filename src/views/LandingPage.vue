<template>
  <div style="padding: 0 20px; display: flex; flex-direction: column">
    <h1 id="title-text">WHAT'S NEW</h1>
    <whats-new-item v-for="post in posts" :key="post.picUrl" :pic-url="post.picUrl" :title="post.title" :body="post.body"/>
    <p>Procuras algo especifico?</p>
    <div
      style="
        display: flex;
        flex-wrap: wrap;
        gap: 10px;
        justify-content: space-around;
        margin-bottom: 32px;
      "
    >
      <small-item v-for="cate in categories" :key="cate.picUrl" :pic-url="cate.picUrl" :title="cate.title" />
    </div>
    <button>Mapa</button>
  </div>
</template>

<script>
import SmallItem from "../components/landing-page/CategoryItem.vue";
import WhatsNewItem from "../components/landing-page/WhatsNewItem.vue";
export default {
  name: "LandingPage",
  components: { WhatsNewItem, SmallItem },
  data() {
    return {
      posts: [
        {
          picUrl: "src/assets/posts/post-1.jpg",
          title: "Campeonato Wave Series",
          body: "A 7º edição das provas de surf regressa para trazer emoção á praia de Leça da Palmeira.",
        },
        {
          picUrl: "src/assets/posts/post-2.jpg",
          title: "Exposição Frida Kahlo",
          body: "Uma exposição imersiva para mergulhar na vida de Frida Kahlo chegou á Alfandega.",
        },
        {
          picUrl: "src/assets/posts/post-3.png",
          title: "Reabertura d’As Marias ",
          body: "Os sabores de sempre numa nova localização em Vila do Conde- agora com vista para o mar.",
        },
      ],
      categories: [
        {
          picUrl: 'src/assets/categories/cate-1.jpg',
          title: 'Restaurantes'
        },
        {
          picUrl: 'src/assets/categories/cate-2.jpg',
          title: 'Praias'
        },
        {
          picUrl: 'src/assets/categories/cate-3.jpg',
          title: 'Cafés'
        },
        {
          picUrl: 'src/assets/categories/cate-4.jpg',
          title: 'Bares'
        },
        {
          picUrl: 'src/assets/categories/cate-5.jpg',
          title: 'Parques'
        },
        {
          picUrl: 'src/assets/categories/cate-6.jpg',
          title: 'Museus'
        }
      ]
    };
  },
};
</script>

<style scoped>
h1 {
  font-size: 30px;
  color: #ff6243;
  text-align: center;
  margin-bottom: 20px;
}

p {
  font-size: 20px;
  color: #ff6243;
  text-align: center;
  margin-top: 40px;
  margin-bottom: 30px;
}

button {
  align-self: center;
  background: #ff0066;
  color: white;
  border: 2px solid #ff0066;
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  border-radius: 30px;
  padding: 8px 80px;
  font-size: 20px;
  margin-bottom: 32px;
}
</style>
