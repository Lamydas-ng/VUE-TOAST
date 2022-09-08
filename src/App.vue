<template>

<button @click="showToast = true">Show Toast</button>

<Toast   
    :show="showToast"
    @hide="showToast = false" 
    message="The message has been sent" 
    type="warning"
    position="bottom-left"
    
   
    />
</template>

<script>
import Toast from "./components/toast/Toast.vue";
export default {
  components: { Toast },
  data: ()=>({
    showToast: false
  }),

};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
