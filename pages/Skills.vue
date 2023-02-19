<template>
    <v-content>
      <v-container id="cont">         
         <br>
         <br>
         <br>
         
         <v-row class="white--text">
         <span class="text-h6 yellow--text text--darken-2 text-decoration-underline"> Overview </span>
         <br>
         <div class="white--text">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laboriosam perferendis ipsum aperiam quos provident excepturi pariatur itaque eius. Nam doloribus ab molestiae exercitationem saepe, natus quas quasi laborum ea commodi!
            <br>
            <br>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur, ea!
            <br>
            <br>
              Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed delectus quis, corporis blanditiis vero nam perferendis repudiandae expedita. Suscipit, corporis?
          </div>  
        </v-row>

         <br>
         <br>

         <span class="text-h6 yellow--text text--darken-2 text-decoration-underline"> My Technology </span>
        <div class="white--text">
            <v-tabs
                v-model="tab"
                color="deep-purple-accent-4"
                align-tabs="end"
                >
                <v-tab >Frontend</v-tab>
                <v-tab >Backend</v-tab>
                <v-tab >Tools</v-tab>
            </v-tabs>
            <br>
            <v-window v-model="tab">
            <v-window-item
                v-for="n in 3"
                v-bind:key="n"
            >
                <v-row v-if="n == 1">
                    <v-col
                    v-for="front in front"
                    v-bind:key="front"
                    cols="6"
                    md="3"
                    >
                    <img :src="'/'+ front + '.png'" />
                    <br>
                    <p class="text-overline ml-3" >{{ front }}</p>
                    </v-col>
                </v-row>

                <v-row v-if="n == 2">
                    <v-col
                    v-for="back in back"
                    v-bind:key="back"
                    cols="6"
                    md="3"
                    >
                    <img :src="'/'+ back + '.png'" />
                    <br>
                    <p class="text-overline ml-3" >{{ back }}</p>
                    </v-col>
                </v-row>

                <v-row v-if="n == 3">
                    <v-col
                    v-for="tools in tools"
                    v-bind:key="tools"
                    cols="6"
                    md="3"
                    >
                    <img :src="'/'+ tools + '.png'" />
                    <br>
                    <p class="text-overline ml-3" >{{ tools }}</p>
                  </v-col>
                </v-row>
            </v-window-item>
            </v-window>

            <div v-motion-pop-bottom>
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Rerum asperiores quae nostrum beatae obcaecati. Aperiam quae deleniti culpa ipsum accusantium, dicta fugiat beatae nam ut vitae velit architecto repellendus dignissimos.
                    Pop from bottom!
            </div>
          

        </div>  
      </v-container>
     </v-content>  
</template>     


<script>
  export default {
    data: () => ({
      tab: null,
      front: ["JavaScript", "HTML", "Nuxt", "VueJS"],
      back: ["MongoDB", "NodeJS", "Python"],
      tools: ["Git", "Linux", "Vim"]
    }),
  }
</script>

<style>
img{
    background-color:antiquewhite;
    border-style: groove;
    border-radius: 1rem;
}
</style>