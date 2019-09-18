<template>
  <section class="section">
    <div class="avatar">
      <img class="avatar-img" src="./../assets/ProfilePic.png" alt="Profile Picture">
    </div>
    <div>
      <h4>Hi, My name is Venkatesh</h4>
      <h5>Brief Introduction About Me</h5>
      <h5>I am a front end developer, Currently I am working @ Zeta India</h5>
    </div>
  </section>
</template>

.<style scoped>
.section {
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
}
.avatar {
  height: 200px;
  width: 150px;
  border-radius: 50px 50px;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
}
.avatar-img {
  max-width: 100%;
  max-height: 100%;
}
</style>
