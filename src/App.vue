<template>
  <div>
    <formCompo></formCompo>
  </div>
</template>

<script>

//importing Form components from components folder
import Form from './components/Form.vue'

export default {
  components: {
    'formCompo': Form
  },
  data () {
    return {
      // developers: [
      //           {name: 'Kingsley Amaechi' , skills: 'Full Stack'},
      //           {name: 'Toheeb Amusa' , skills: 'Front-End'},
      //           {name: 'Oderinde Bukola' , skills: 'App Developer'},
      //           {name: 'Ajani Oluwafemi' , skills: 'Back-end'},
      //           {name: 'Lawrence Olaitan' , skills: 'Database'},
      //           {name: 'Tijani Idris' , skills: 'Full Stack'},
      //           {name: 'Okoye Destiny' , skills: 'Front-End'},
      //           {name: 'Ibeh Favour' , skills: 'Full Stack'},
      // ],
      // copyright: 'Copyright.',
      // copyrightCont: 'All Right Reserved. Brain.js 2019',
      // who: 'I am Brain.js'
    }
  }, 
  methods: {
    
  }, 
  computed: {

  }
}
</script>
<style scoped>
  img{
    padding: 10px;
  }
  div #firstHeaderBackground{
    background-color: lightgreen;
    padding-bottom: 20px;
    margin-bottom: 20px;
  }
</style>
