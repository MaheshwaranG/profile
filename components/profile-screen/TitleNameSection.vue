<template>
  <div
    class="w-full p-6 bg-white overflow-hidden shadow-md sm:rounded-lg relative flex flex-wrap md:flex-nowrap gap-1"
  >
    <div class="rounded-2xl md:rounded-full bg-red-100 bg-opacity-25 p-8 ml-2 mt-2 flex w-full md:w-max items-center justify-center" style="height: max-content">
      <a-avatar id="user-intro-photo"
        :size="140"
        :style="{ verticalAlign: 'middle' }"
        src="/photos/maheshwaran.jpg"
        alt="Maheshwaran Gopal"
        class="scale-250"
      >
      </a-avatar>
    </div>
    <div class="m-4 flex flex-col justify-center w-full md:w-max md:justify-start relative gap-4">
      <h3 class="text-4xl font-serif font-bold tracking-wide text-black truncate max-w-26rem text-center md:text-left ">
        Maheshwaran G 
      </h3>
      <div class="text-2xl flex justify-center md:justify-start">
        <a-tag color="cyan">
             <i class="fa-solid fa-briefcase fa-xl"></i>
          End to End Software Developer</a-tag
        >
      </div>
      <div>
        <ContactDetails />
      </div>
    </div>
  </div>
</template>
<script>
import ContactDetails from "./ContactDetails.vue"
export default {
  components: {
    ContactDetails
  }
}
</script>
<style scoped>
/* a >>> b { color : red; }
/deep/ a b { color : red; }
a::v-deep b { color : red; } */
 #user-intro-photo::v-deep > img {
  transform: scale(3);
}
</style>