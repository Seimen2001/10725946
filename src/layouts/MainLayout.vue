<template>
  <div class="q-pa-md">
    <div class="q-gutter-y-md" style="max-width: 100vw">
      <q-card>
        <q-tabs
          v-model="tab"
          dense
          class="bg-grey-2 text-grey-7"
          active-color="primary"
          indicator-color="purple"
          align="justify"
        >
          <q-tab v-model="tab" no-caps  name="HomePage" label="HomePage" />
          <q-tab v-model="tab" no-caps  name="AboutMe" label="AboutMe" />
          <q-tab v-model="tab" no-caps  name="MySkills" label="MySkills" />
          <q-tab v-model="tab" no-caps  name="Education" label="Education" />
          <q-tab v-model="tab" no-caps  name="Hobbies" label="Hobbies" />
        </q-tabs>

        <q-tab-panels v-model="tab" animated class="bg-dark text-grey-5">
          <q-tab-panel name="HomePage">
          <div class="home-container">
          <div class="image-and-content-container">
      <!-- Left side: Image -->
          <div class="image-container">
          <img class="centered-image" src="../assets/seimen.jpg" alt="My Image" />
          </div>
      <!-- Right side: Content -->
          <div class="content-container">
          <h4 style="margin: 10px">Ale Seimen</h4>
          <div class="info">
          <b>Contact information:</b><br>
          aleseimen001@gmail.com<br>
          +91 8897520952<br>
          Uppal, Hyderabad<br>
          www.linkedin.com/in/ale-seimen-a80165186<br>
          </div>
          </div>
          </div>
          </div>
          </q-tab-panel>

          <q-tab-panel name="AboutMe">
            <div class="text-h6">About me</div><br>
            Hello, I'm a dedicated trainee software engineer based in the vibrant city of Hyderabad.Currently, I am excited to be a part of the LTIMindtree, where I'm embarking on a journey of continuous learning and growth in the world of software development. With a deep passion for coding and problem-solving, I thrive on the challenges and complexities of the tech world.<br> My journey began with a strong educational foundation in computer science, and I'm eager to apply my skills to develop innovative solutions and contribute to meaningful projects. <br>I'm a firm believer in the power of tech-nology to make a positive impact, and I'm committed to becoming a valuable as-set in this ever-evolving field.
            </q-tab-panel>

          <q-tab-panel name="Education">
          <div class="text-h6">My Education</div><br>
          <div class="text-h6">Bachelor Of Technology</div><br>
          Anurag Group of Institutions (2019-2023)<br>
          CGPA - 8.91 <br>
          Hyderabad <br><br>
          <div class="text-h6">Intermediate</div><br>
          Sri Chaitanya Junior Kalasala (2017-2019) <br>
          Aggregate - 93.7% <br>
          Hyderabad <br><br>
          <div class="text-h6">SSC</div><br>
          Sri Sai Model High School <br>
          CGPA - 9.7 <br>
          Hyderabad <br><br>
          
          </q-tab-panel>

            <q-tab-panel name="MySkills">
            <div class="text-h6">Technical Skills</div><br>
            <div>
            <p>As a trainee at LTIMindtree, I have had the privilege of honing my technical skills through a structured and comprehensive training program. My educational background in computer science provided me with a solid founda-tion, and my time at LTIMindtree has allowed me to further refine and expand my skill set. I have gained proficiency in following areas:</p>
            * Windows<br>
            * Linux<br>
            * Networks<br>
            * Virtualization<br>
            * Git, Github<br>
            * SpringBoot, Java<br>
            * Vue JS, Quasar<br>
            * ArangoDB<br>
            * Spark and Kafka<br>
            * Python wityh Data Analysis<br>
            * AI & ML<br>
            </div>
            </q-tab-panel>
            <q-tab-panel name="Hobbies">
            <div class="text-h6">My Hobbies</div><br>
             <h6>I love to explore various painting styles, from vibrant abstracts to intricate landscapes, and my sketchbook is filled with potraits and scenes from my everyday life. Here are a few samples of my work:</h6>
             <div class="image-container">
             <img class="centered-image" src= "../assets/1.jpg" alt="My Image 1" width="300" height="300" />
            <img class="centered-image" src= "../assets/2.jpg" alt="My Image 2" width="300" height="300" />
              </div>
            </q-tab-panel>
        </q-tab-panels>
      </q-card>
    </div>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      tab: ref('HomePage')
    }
  }
}
</script>

<style scoped>
/* Style for the overall container */
.q-pa-md {
  /* display: ; */
  justify-content: center;
  align-items: center;
  height: 100vh; /* Centers content and makes it fit the screen */
}

.image-and-content-container {
  display: flex;
  align-items: center;
}


.content-container {
  /* flex: 3;  */
  display: flex;
  /* max-width: 50%; */
  /* padding: 10px;  */
  margin-left: 30px;
}

.info{
  padding-left: 35px;
}
.image-container {
  display: flex;
  align-items: center;
 
}

.centered-image {
  max-width: 50%; /* Adjust the width of each image as needed */
  margin-left: 30px;
}
</style> 


