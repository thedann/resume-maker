<template>
  <div class="about">
    <h1>This is an about page</h1>
    <button v-on:click="click">click me</button>
  </div>
</template>

<script>
export default {
  name : 'About',
  methods: {
    click : () => {
      alert("click");
      getData();
    }
  }
}

const getData = async () => {
  const response = await fetch('http://localhost:5000/phone');
  const myJson = await response.json();
  console.log(myJson);
}
</script>
