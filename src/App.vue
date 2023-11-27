<template>
    <MainContent />
    <AboutMe />
    <EducationExperience />
    <SkillsPortfolio />
    <ContactMe />
</template>

<script>
import MainContent from "./components/MainContent.vue";
import AboutMe from "./components/AboutMe.vue";
import EducationExperience from "./components/EducationExperience.vue";
import SkillsPortfolio from "./components/SkillsPortfolio.vue";
import ContactMe from "./components/ContactMe.vue";
export default {
    name: "App",
    components: { MainContent, AboutMe, EducationExperience, SkillsPortfolio, ContactMe },
};
</script>

<style>
body {
    margin: 0;
}
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    display: flex;
    flex-direction: column;
    background-color: #050505;
    color: #ffffff;
    user-select: none;
}
#app > * {
    height: 100vh;
}

::-webkit-scrollbar {
    width: 8px;
}

::-webkit-scrollbar-track {
    background: #3f3f3f;
}

::-webkit-scrollbar-thumb {
    background: #e2b714;
}

::-webkit-scrollbar-thumb:hover {
    background: #f9e18b;
}

::-webkit-scrollbar-thumb:active {
    background: rgb(255, 200, 0);
}
</style>
