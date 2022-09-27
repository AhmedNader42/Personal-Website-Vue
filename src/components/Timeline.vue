<template>
  <div style="margin: 10px; padding: 10px;">
    <vue-timeline-update
      :date="new Date('2015-06-01')"
      title="Computer Science - Cairo University"
      description="It was the start of my lifelong learning journey that sparked my love for programming. I graduated in 2019 with a grade of Very Good."
      category="Education"
      color="blue"
      icon=""
      class="text-primary"
    />

    <vue-timeline-update
      :date="new Date('2017-08-01')"
      title="(iOS Developer) - KickstartInteractive, Cairo - Egypt"
      description="My first professional job in the summer of 2017. While there I worked on VKader as an iOS developer. A great learning experience and a challenging project in terms of scale and size. I gained a lot of experience over the course of completing the App."
      category="Full-Time"
      color="purple"
      icon=""
      class="text-primary"
    />

    <vue-timeline-update
      :date="new Date('2018-08-01')"
      title="(iOS Developer) IntCore, Cairo - Egypt"
      description="Next summer I was part of the IntCore iOS team working on SnapCars which was a different experience. It was a collaborative experience that taught me how to pay attention to the details no matter how small."
      category="Full-Time"
      color="purple"
      icon=""
      class="text-primary"
    />

    <vue-timeline-update
      :date="new Date('2020-06-01')"
      title="(Software Developer) Research Center Egyptian Armed Forces, Cairo - Egypt"
      description="From June 2020 until June 2021 I was doing my mandatory military service. I was lucky enough to be in a place where programming was a viable option. I was mostly working with web technologies such as HTML, CSS, Javascript and both SQL and NoSQL databases. I worked on different kinds of classified projects it helped develop my software engineering skills and taught me a lot about handling complexity. It was a tough environment with lots of tasks and pressure to get things out quickly and correctly. I learned constant iterations are the best way to improve a software project and also a lot of team working skills and other soft skills as well as technical."
      category="Full-Time"
      color="red"
      icon=""
      class="text-primary"
    />

    <vue-timeline-update
      :date="new Date('2021-09-29')"
      title="(SAS Technical consultant) Data Science MiddleEast, Cairo - Egypt"
      description="DataScience is a SAS silver partner using SAS data management tools. I received training for SAS tools and SAS programming. I also received intense Database training. I still work with Datascience working on contracting projects."
      category="Full-Time"
      color="red"
      icon=""
      class="text-primary"
    />

    <vue-timeline-update
      :date="new Date('2022-01-19')"
      title="(Data Engineer) Abu Dhabi Police ICT, Abu Dhabi - United Arab Emirates"
      description="One of the most important contract for Datascience was AbuDhabi Police's investigation software which is a huge scale project requiring deep expertise and technical knowledge to handle the Big Data and creating ETL Pipelines from scratch while also making sure the data quality and the correct data model."
      category="Full-Time (Contract)"
      color="red"
      icon=""
      class="text-primary"
      is-last
    />
  </div>
</template>

<script>
export default {
  name: "Timeline",
  data: () => ({
    years: [
      {
        color: "cyan",
        year: "2015",
        entity: "(Computer Science - Cairo University)",
        experience:
          "It was the start of my lifelong learning journey that sparked my love for programming. I graduated in 2019 with a grade of Very Good.",
      },
      {
        color: "green",
        year: "2017",
        entity: "(iOS Developer - KickstartInteractive)",
        experience:
          "My first professional job in the summer of 2017. While there I worked on VKader as an iOS developer. A great learning experience and a challenging project in terms of scale and size. I gained a lot of experience over the course of completing the App.",
      },
      {
        color: "pink",
        year: "2018",
        entity: "(iOS Developer - IntCore)",
        experience:
          "Next summer I was part of the IntCore iOS team working on SnapCars which was a different experience. It was a collaborative experience that taught me how to pay attention to the details no matter how small.",
      },
      {
        color: "amber",
        year: "2019",
        entity: "(Computer Science - Cairo University)",
        experience:
          "The year I graduated from college. I was working on my graduation project with 4 other teammates. The idea was to predict whether the skin shown in the photo was benign or malignant of skin cancer. We trained a model on a dataset containing 55+GB of Images.",
      },
      {
        color: "orange",
        year: "2021",
        entity: "(Software Engineer, Research Center Egyptian Armed Forces)",
        experience:
          "From June 2020 until June 2021 I was doing my mandatory military service. I was lucky enough to be in a place where programming was a viable option. I was mostly working with web technologies such as HTML, CSS, Javascript and both SQL and NoSQL databases. I worked on different kinds of classified projects it helped develop my software engineering skills and taught me a lot about handling complexity. It was a tough environment with lots of tasks and pressure to get things out quickly and correctly. I learned constant iterations are the best way to improve a software project and also a lot of team working skills and other soft skills as well as technical.",
      },
      {
        color: "orange",
        year: "2021",
        entity: "(SAS Technical consultant, Data Science MiddleEast)",
        experience:
          "DataScience is a SAS silver partner using SAS data management tools. I received training for SAS tools and SAS programming. I also received intense Database training. I still work with Datascience working on contracting projects.",
      },
      {
        color: "violet",
        year: "2022",
        entity: "(Data Engineer, Abu Dhabi Police ICT)",
        experience:
          "One of the most important contract for Datascience was AbuDhabi Police's investigation software which is a huge scale project requiring deep expertise and technical knowledge to handle the Big Data and creating ETL Pipelines from scratch while also making sure the data quality and correctness while also optimizing database for performance.",
      },
    ],
  }),
}
</script>
