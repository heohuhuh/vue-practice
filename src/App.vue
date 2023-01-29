<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <div>
    <h4 class="red" :style="Style">{{ products[0] }}</h4>
    <p>{{ price[0] }} 만원</p>
  </div>
  <div>
    <h4>{{ products[1] }}</h4>
    <p>{{ price[1] }}만원</p>
    <!--data().price1 이런거 아님-->
  </div>
  <div>
    <h4>{{ products[2] }}</h4>
    <p>{{ price[2] }} 만원</p>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      price: [70, 80, 90],
      Style: "color:blue",
      products: ["역삼동원룸", "천호동원룸", "마포구원룸"],
    };
  },
  components: {},
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
