<template>
  <div>
    <h1 id="projects">Projects</h1>
    <div class="container">
      <div class="row">
        <div
          class="col-12 col-md-4 proj"
          v-for="project in projects"
          :key="project"
        >
          <card
            :title="project.title"
            :description="project.description"
            :image="project.image"
            :frameworks="project.frameworks"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Card from "./CardComponent.vue";

export default {
  name: "project",
  components: { Card },
  data() {
    return {
      projects: [
        {
          title: "xDev",
          description:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book",
          image: "./images/xdev.png",
          frameworks: [
            { frame: "./images/laravel.png" },
            { frame: "./images/vue.png" },
            { frame: "./images/mysql.png" },
          ],
        },
        {
          title: "Todo List",
          description:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book",
          image: "./images/todo.jpg",
          frameworks: [{ frame: "./images/vue.png" }],
        },
        {
          title: "OSRS Bot",
          description:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book",
          image: "./images/osrs.jpg",
          frameworks: [
            { frame: "./images/node.png" },
            { frame: "./images/robot.png" },
          ],
        },
        {
          title: "Rest API",
          description:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book",
          image: "./images/restapi.png",
          frameworks: [
            { frame: "./images/node.png" },
            { frame: "./images/mongo.png" },
          ],
        },
        {
          title: "Ticket Manager",
          description:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book",
          image: "./images/ticket.png",
          frameworks: [{ frame: "./images/csharp.png" }],
        },
        {
          title: "iZiBiZi",
          description:
            "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book",
          image: "./images/izibizi.png",
          frameworks: [{ frame: "./images/php.png" }],
        },
      ],
    };
  },
};
</script>

<style>
img {
  margin: 2px;
}
.proj {
  padding-top: 2%;
  padding-bottom: 2%;
}
</style>