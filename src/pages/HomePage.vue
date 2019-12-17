<template>
  <div class="container mx-auto">
    <AppTitle :title="'Taufiq Rohman'" :subtitle="'Frontend &amp; Mobile Developer'" />

    <div class="container p-4 pt-6 border-t-2 border-color-green border-dashed mt-8">
      <div class="flex-column">
        <Contact
          :icon="'mail'"
          :name="'taufiqrohman@outlook.com'"
          :link="'mailto:taufiqrohman@outlook.com'"
          color="indigo"
        />
        <Contact
            icon="linkedin"
            name="LinkedIn"
            link="https://www.linkedin.com/in/taufiq-rohman-41a707b9/"
            color="teal"
        />
        <Contact
            icon="twitter"
            name="Follow Me @taufiqroh"
            link="https://twitter.com/taufiqroh"
            color="blue"
        />
      </div>
    </div>

    <div class="container p-4 border-t-2 border-b-2 border-color-indigo border-dashed my-4">
      <div class="flex-row">
          <Skill title="Laravel" :level="90" color="red" />
        <Skill :title="'ReactJS'" :level="80" :color="'indigo'" />
        <Skill :title="'VueJS'" :level="70" :color="'green'" />
        <Skill :title="'Flutter'" :level="60" />
        <Skill :title="'React Native'" :level="80" :color="'purple'" />
      </div>
    </div>
  </div>
</template>

<script>
import Skill from "../components/Skill";
import AppTitle from "../components/AppTitle";
import Contact from "../components/Contact";

export default {
  name: "HomePage",
  components: {
    Skill,
    AppTitle,
    Contact
  }
};
</script>