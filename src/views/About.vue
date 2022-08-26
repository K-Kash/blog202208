<template>
  <div class="about">
    <img class="logo" src="https://k-kash.s3.us-west-1.amazonaws.com/logo-kiku.png">
    <h2>KASH-KIKU</h2>
    <p>
    ツーリングが趣味の管理人が旅や愛犬の記録を備忘録として、発信している趣味ブログです。
    </p>
    <v-btn icon href="https://www.instagram.com/kash.kiku" color="#C13584">
      <v-icon>mdi-instagram</v-icon>
    </v-btn>
  </div>
</template>

<style>

.about {
  text-align: center;
}

img.logo {
    width: 40%;
    height: 40%;
  }

p {
  margin: 32px;
}

.mdi-instagram {
  background: radial-gradient(
    circle at 30% 107%,
    #fdf497 0%,
    #fdf497 5%,
    #fd5949 45%,
    #d6249f 60%,
    #285aeb 90%
  );
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
}


</style>
