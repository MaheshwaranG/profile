<template>
  <div class="p-6 bg-white overflow-hidden w-full">
    <h2 class="text-xl mb-3 font-serif font-bold">Experience</h2>
    <div id="experience">
      <a-timeline>
        <a-timeline-item>
          <template #dot>
            <TimelineDot
              :iconClass="o4s.dot.iconName"
              parentStyle="--fa-animation-duration:3s;--fa-beat-scale:1.1"
              parentClass="fa-beat"
            />
          </template>
          <template>
            <TimelineDetails
              :title="o4s.title.name"
              :institute="o4s.institute"
              :place="o4s.place"
              :timeline="o4s.timeline"
              :details="o4s.details"
              listClass="experience"
            />
          </template>
        </a-timeline-item>
        <a-timeline-item>
          <template #dot>
            <TimelineDot
              :iconClass="sentisum.dot.iconName"
              parentStyle="--fa-animation-duration:3s;--fa-beat-scale:1.1"
              parentClass="fa-beat"
            />
          </template>
          <template>
            <TimelineDetails
              :title="sentisum.title.name"
              :institute="sentisum.institute"
              :place="sentisum.place"
              :timeline="sentisum.timeline"
              :details="sentisum.details"
              listClass="experience"
            />
          </template>
        </a-timeline-item>
        <a-timeline-item>
          <template #dot>
            <TimelineDot
              :iconClass="ivtl.dot.iconName"
              parentStyle="--fa-animation-duration:3s;--fa-beat-scale:1.1"
              parentClass="fa-beat"
            />
          </template>
          <template>
            <TimelineDetails
              :title="ivtl.title.name"
              :institute="ivtl.institute"
              :place="ivtl.place"
              :timeline="ivtl.timeline"
              :details="ivtl.details"
              listClass="experience"
            />
          </template>
        </a-timeline-item>
      </a-timeline>
    </div>
  </div>
</template>
<script>
import TimelineDetails from "./TimelineDetails.vue";
import TimelineDot from "./TimelineDot.vue";
export default {
  name: "Experience",
  components: {
    TimelineDetails,
    TimelineDot,
  },
  data: () => ({
    o4s: {
      dot: {
        iconName: "fa-server",
      },
      title: {
        name: "Software Engineer - Backend",
      },
      institute: {
        icon: `<i class="fa-solid fa-code"></i>`,
        name: "O4S",
      },
      place: {
        icon: `<i class="fa-solid fa-location-dot"></i>`,
        name: "Gurgaon - Hybrid",
      },
      timeline: {
        icon: `<i class="fa-solid fa-calendar-days"></i>`,
        name: "Feb 2022 - Current",
      },
      details: [
        "Supporting production fire issues",
        "Working on O4S serialization application",
        "Working on edge application - bug fix, setup, deployment",
        "Developed O4S admin application",
        "Created guideline and best pratices for frontend development when revamp the new designs",
        "Guiding Juniors for development of the product",
        "Have been working closely with product team to deliver product goals and giving input for improvement",
        "Volunteeringly doing engineering planing and helping others to deliver feature fast.",
      ],
    },
    sentisum: {
      dot: {
        iconName: "fa-laptop-code",
      },
      title: {
        name: "Member Of Technical Staff - Full Stack Developer",
      },
      institute: {
        icon: `<i class="fa-solid fa-code"></i>`,
        name: "SentiSum",
      },
      place: {
        icon: `<i class="fa-solid fa-location-dot"></i>`,
        name: "Bengaluru - Remote",
      },
      timeline: {
        icon: `<i class="fa-solid fa-calendar-days"></i>`,
        name: "Feb 2021 – Feb 2022",
      },
      details: [
        "Worked in an analytical application with React, Python, Java, Spring, \
        Django, PostgreSQL, Elastic search, Integrations, ETL tasks.",
        "Supported and Maintained multiple services especially frontend, admin \
          services. I was the only one who completely led the frontend from \
          development to testing of the application.",
        "Given support and guide to use existing system model to support new \
          features without altering model.",
        "Improved dashboard performance and user experience by introducing \
          configurable components based on environment and runtime \
          configuration, which also helps to easily adapt new changes. Used code \
          splitting concept to minimize bundle size, git actions for smooth \
          deployment in different environments.",
        "Implemented deep search, views, different metric dimensions and some \
          more to show granular details for root cause analysis.",
        "Identified bottlenecks, pain points, and bugs in the application and \
          immediately took remedies to fix issues.",
        "Worked with different third-party apps for Integration and implemented \
          Oauth flow and supported ETL tasks.",
      ],
    },
    ivtl: {
      dot: {
        iconName: "fa-building-lock",
      },
      title: {
        name: "Junior Engineer - Full Stack Developer",
      },
      institute: {
        icon: `<i class="fa-solid fa-code"></i>`,
        name: "IVTL Infoview",
      },
      place: {
        icon: `<i class="fa-solid fa-location-dot"></i>`,
        name: "Chennai - Remote",
      },
      timeline: {
        icon: `<i class="fa-solid fa-calendar-days"></i>`,
        name: "Jul 2017 – Jan 2021",
      },
      details: [
        "Worked in a Mail application project with MongoDB, Node js, React,\
          Elastic search, Redis, Python, Docker.",
        "Improved user experience by implementing advanced search.",
        "Identified bugs in code and improved system performance a lot with\
          very minimal response time (100ms) and reduced production server\
          cost by reconfiguring server architecture.",
        "Worked on system design based on the requirement, implemented a\
          model, distributed system design to achieve a highly available and\
          scalable system, implemented CI/CD pipeline to deploy an application\
          and supported for maintenance.",
        "Great exposures on file storage management and security\
          practices(XSS, CORS, HTTPS, XSRF, DoS, and more).",
        "Follows mail standard protocols (SMTP, POP3, IMAP) for\
          implementation.",
        "Worked on the various environments from the development\
          environment to the Production environment to deliver an application.",
        "Worked on various tools like Postman, Jenkins, cloud services Like\
          AWS (S3, EC2 Instance), shell commands, scheduling jobs for data migration, backup, data analytics.",
        "Besides, I have supported Calendar service, App Generator projects.",
        "Worked in an ERP product development in SCM division with spring framework, Maven,\
          google closure, and SQL.",
        "In addition, analyzed the existing code and worked with a team members to fix DevOps bugs and\
          executed all test cases and delivered on time."
      ],
    },
  }),
};
</script>

<style scoped lang="scss">
::v-deep(.experience) {
  li::first-letter {
    // @apply text-blue-800;
    @apply text-base;
    // @apply font-bold;
    // @apply mr-0.5;
  }
}
</style>