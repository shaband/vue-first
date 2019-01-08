<template>
  <div>
    <div v-for="(user,key) in users" :key="key" class="card" @click="user.show=!user.show">
      <img src="https://www.w3schools.com/howto/img_avatar.png" alt="Avatar" style="width:100%">
      <div class="container">
        <h4>
          <b>{{user.name}}</b>
        </h4>
        <p v-show="user.show">{{user.job}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      users: [
        { name: "mahmoud", job: "dev" ,show:false},
        { name: "hazem", job: "doc" ,show:false},
        { name: "hazem", job: "lol" ,show:false}
      ]
    };
  }
};
</script>
<style scoped>
.card {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  transition: 0.3s;
  width: 30%;
  display: inline-block;
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
}

.container {
  padding: 2px 16px;
}
</style>
