<template>
    <div class="pl-2 flex flex-col gap-2">
              <h2 class="text-base font-serif font-medium">
                {{title}}
              </h2>
              <div class="flex justify-between mr-1 flex-wrap gap-2">
              <div class="flex gap-2">
                <a-tag color="cyan">
                  <!-- <component :is="institute.icon" />  -->
                   <span v-html="institute.icon"></span>
                  <span class="text-sm ml-1">{{institute.name}}</span>
                </a-tag>
                <a-tag color="cyan">
                  <!-- <component :is="institute.icon" />  -->
                   <span v-html="place.icon"></span>
                  <span class="text-sm ml-1">{{place.name}}</span>
                </a-tag>
              </div>
              <div>
                <span v-html="timeline.icon"></span>
                <span class="font-semibold">{{timeline.name}}</span>
              </div>
               </div>
               <div>
                <ul :class="listClass">
                    <li v-for="(desc, index) in details" :key="index" class="my-1.5 mx-1">
                        {{desc}}
                    </li>
                </ul>
               </div>
            </div>
</template>
<script>
export default {
    name: "TimelineDetails",
    props: ["title", "institute", "place", "timeline", "details", "listClass"]
}
</script>