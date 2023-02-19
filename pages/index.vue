 <template>
     <v-main>
      <v-container id="cont">
         <v-row>
            <div>
               <typewriters/>
            </div>
         </v-row>
         <v-row class="white--text">
         <span class="text-h4 yellow--text text--darken-2">Albert Attakora Frimpong</span>
         <div class="white--text">
            Full Stack Web Developer/ Mathematics Teacher/ Electronics Hobbist
         </div>
         </v-row>
         
         <br>
         <br>
         <br>
         
         <v-row class="white--text">
         <span class="text-h6 yellow--text text--darken-2 text-decoration-underline">Professional Background</span>
         <br>
         <div class="white--text">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laboriosam perferendis ipsum aperiam quos provident excepturi pariatur itaque eius. Nam doloribus ab molestiae exercitationem saepe, natus quas quasi laborum ea commodi!
            <br>
            <br>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur, ea!
         </div>  
         </v-row>

         <v-row class="white--text">
         <span class="text-h6 yellow--text text--darken-2 text-decoration-underline">Bio</span>
         <br>
         <div class="white--text">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laboriosam perferendis ipsum aperiam quos provident excepturi pariatur itaque eius. Nam doloribus ab molestiae exercitationem saepe, natus quas quasi laborum ea commodi!
            <br>
            <br>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur, ea!
         </div>  
         </v-row>

         <v-row class="white--text">
         <span class="text-h6 yellow--text text--darken-2 text-decoration-underline">Journey</span>
         <br>
         <div class="white--text">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Laboriosam perferendis ipsum aperiam quos provident excepturi pariatur itaque eius. Nam doloribus ab molestiae exercitationem saepe, natus quas quasi laborum ea commodi!
            <br>
            <br>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Consectetur, ea!
         </div>  
         </v-row>
      </v-container>
     </v-main> 
</template>     

<script>
   import typewriters from '../components/typewriter'

   export default {
        components: {
         typewriters
        },
    }
</script>



<style>
#cont{
   background: midnightblue;
   text-underline-position: under;  
}

</style>