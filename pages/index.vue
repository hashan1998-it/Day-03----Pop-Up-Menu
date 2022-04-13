<template>
  <div class="d-flex justify-content-center align-items-center vh-100 flex-column">
    <MainContainer  @showPop="showPop"/>
    <PopUp :class="showState ? 'd-flex' : 'd-none' " @showPop="showPop" />
  </div>
</template>

<script>
import MainContainer from '~/components/Main Container/MainContainer.vue'
import PopUp from '~/components/Pop Up/PopUp.vue'
export default {
  name: 'IndexPage',
  components:{
    MainContainer,PopUp
  },
  data(){
    return{
      showState: false
    }
  },
  methods:{
    showPop(){
      if(this.showState == false){
        this.showState = true
      }
      else{
        this.showState= false
      }
    }
  }
}
</script>

<style scoped>

</style>
