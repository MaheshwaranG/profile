<template>
      <div
              :class='["p-1.5 bg-blue-200 flex items-center justify-center rounded-2xl shadow-md shadow-gray-300", parentClass]'
              :style='parentStyle'
            >
              <div
                class="ring-2 ring-blue-500 p-0.5 flex items-center justify-center h-5 w-5 rounded-2xl"
              >
                <i :class='["fa-solid fa-sm text-black", iconClass]'></i>
              </div></div
          >
</template>
<script>
export default {
    name: 'TimelineDot',
    props: ['iconClass', 'parentStyle', 'parentClass'],
}
</script>