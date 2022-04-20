<template>
  <div style="margin-bottom: 80px;">
    <h1>Hey!</h1>

    <div class="paragraph">
      <div>
        I'm <strong>Ben Holland</strong>, an indie & freelance game developer.<br/>
        I make some pretty cool stuff. This is the place to see it all!
      </div>

      <div style="margin-top: 20px;">I've worked on  <router-link to="/game-projects">Steam Games</router-link>, on some <router-link to="/other-projects">Random Projects</router-link>, and took part in <router-link to="/resume">A Few Game Jams</router-link> as well.</div>

      <div style="margin-top: 40px;">I'm <strong>currently looking for freelance projects</strong>. You can reach me at <a href="mailto:fifthedgestudios@gmail.com">fifthedgestudios@gmail.com</a> or <router-link to="/contact">through here</router-link>.</div>
    </div>

    <div >
      <img src="img/avatar.png" alt="Avatar of Ringo" class="photo"/> 
    </div>

    <div style="clear:both"></div>

  </div>
</template>

<style scoped>
.paragraph {
  max-width: 700px;
  margin-bottom: 20px;
}

.photo {
  width:400px; 
  height:auto;
  border-radius: 100%;
}

@media only screen and (min-width: 620px){
  .paragraph {
    float: left;
  }

  .photo {
    float: left;
    padding: 10px;
    padding-left: 80px;
  }
}

</style>