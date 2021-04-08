<template>
  <div class="home">
    <ul>
      <li>
        <router-link :to="{ name: 'Member' , params: { id: 1} }">
          1へ進む
        </router-link>
      </li>
      <li>
        <router-link :to="{ name: 'Member' , params: { id: 2} }">
          2へ進む
        </router-link>
      </li>
      <li>
        <router-link :to="{ name: 'Member' , params: { id: 3} }">
          3へ進む
        </router-link>
      </li>
    </ul>
  </div>
</template>

<style scoped>
ul {
  padding:0px;
}
li{
  list-style:none;
}
</style>

<script>
export default{
  methods:{
    transition(){
      this.$router.push({name: "Member" , params: { id: 1} });
      this.$router.push({name: "Member" , params: { id: 2} });
      this.$router.push({name: "Member" , params: { id: 3} });
    } 
  }
};

</script>
