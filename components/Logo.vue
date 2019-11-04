<template>
  <div class="wrapper">
    <img
      class="logo"
      alt="Logo"
      src="/logo.png"
    >
    <div class="title">
      <h2>NOANSA</h2>
      <p>coffee roasters</p>
    </div>
  </div>
</template>

<style scoped>

.logo{
  width: 30px;
  height: 30px;
}

.title{
  margin-left: 5px;
  padding-left: 2px;
  justify-content: space-around
}

h2{
  text-transform:uppercase;
  font-size: 1.2rem;
}

p{
  font: .6rem sans-serif;
  text-transform:uppercase
}

.wrapper{
  display: flex;
  flex-direction: row;
}

</style>
