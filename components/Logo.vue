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
  width: 40px;
  height: 40px;
}

.title{
  margin-left: 5px;
  padding-left: 2px;
}

h2{
  text-transform:uppercase;
  font-size: 1rem;
}

p{
  font: .4rem sans-serif;
  text-transform:uppercase
}

.wrapper{
  display: flex;
  flex-direction: row;
}

</style>
