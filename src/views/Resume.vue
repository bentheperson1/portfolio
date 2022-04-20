<template>
  <div>
    <h1>Resume</h1>

    <div class="paragraph">
      I'm <strong>Ben Holland</strong>, an indie & freelance game developer.
      <br /><br />I've been doing game development in general for about 4-5 years now.
      <br />My main game engine of choice is GameMaker/GameMaker Studio 2. I also have substantial experience with Unity & Godot.<br/>
      <br />I'm currently 15 and I've been programming and doing game development since I was about 11. 
    </div>
    <div>
      <div class="photo">
        <img src="img/resume-avatar.png" alt="Photo of Ben" style="width: 300px; height: auto; margin-bottom: 5%; border-radius: 5%;" />
        <h3 style="text-align: center;">^ Me ^</h3>
      </div>
      <br />
    </div>

    <div style="clear:both"></div>

    <div class="full-content">
      <h2>Work experience</h2>

      <h3>Fifth Edge Studios</h3>
      <h4>2018-Present</h4>

      <div>My personal development studio that I release all of my projects under.</div>

      <div class="tech-stack">GameMaker, Unity, Python, Godot, Aseprite</div>

      <h2>Skills</h2>

      <div class="skill-set">
        <h3>Game Development</h3>
        <SkillRate name="GameMaker" :rate="5" />
        <SkillRate name="Unity" :rate="4" />
        <SkillRate name="Godot" :rate="3" />
      </div>

      <div class="skill-set">
        <h3>General Programming</h3>
        <SkillRate name="HTML+CSS" :rate="5" />
        <SkillRate name="Git" :rate="3" />
        <SkillRate name="Python" :rate="4" />
        <SkillRate name="Problem Solving" :rate="4" />
      </div>
      <div style="clear:both" />

      <h2>Education</h2>

      <h4>Bailey JR High - 2021</h4>
      <h4>Arlington High School - 2025</h4>
      
      <h2>Languages</h2>

      <h3>English</h3>
      <div>I'm a native English speaker.</div>

      <h3>French</h3>
      <div>I really only know the basics.</div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import SkillRate from "@/components/SkillRate.vue";

export default Vue.extend({
  name: "Resume",
  components: {
    SkillRate,
  },
});
</script>

<style scoped>
h2 {
  font-weight: 100;
  font-size: 2em;
  margin: 0px;
  padding: 0px;
  padding-top: 50px;
}
h3 {
  font-weight: 100;
  font-size: 1.6em;
  margin: 0px;
  padding: 0px;
  padding-top: 30px;
}
h4 {
  font-weight: 100;
  font-size: 1.3em;
  margin: 0px;
  padding: 0px;
  padding-top: 15px;
  font-style: italic;
}

.paragraph {
  max-width: 700px;
}

.download-link {
  float:left;
  margin-right: 50px;
}

.full-content div {
  max-width: 800px;
}

.skill-set h3 {
  padding-bottom: 10px;
}

.photo img {
  height: 300px;
  width: 300px;
}

.tech-stack {
  font-style: italic;
}

.photo {
  text-align: center;
}

@media only screen and (min-width: 620px){
  .paragraph {
    float: left;
  }

  .photo {
    float: left;
    padding: 30px;
    padding-left: 80px;
  }

  .skill-set {
    float: left;
    padding-right: 60px; 
  }
}
</style>