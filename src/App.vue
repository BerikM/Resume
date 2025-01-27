<script setup lang="ts">
import ResumeAbout from "@/components/ResumeAbout.vue";
import ResumeExperience from "@/components/ResumeExperience.vue";
import ResumeHeader from "@/components/ResumeHeader.vue";
import ResumeLanguages from "@/components/ResumeLanguages.vue";
import ResumeName from "@/components/ResumeName.vue";
import ResumeOverview from "@/components/ResumeOverview.vue";
import ResumePortfolio from "@/components/ResumePortfolio.vue";
import ResumeSkills from "@/components/ResumeSkills.vue";
</script>

<template>
    <ResumeHeader></ResumeHeader>
    <ResumeName></ResumeName>
    <ResumeAbout id="about"></ResumeAbout>
    <ResumeOverview></ResumeOverview>
    <ResumeSkills id="skills"></ResumeSkills>
    <ResumeLanguages></ResumeLanguages>
    <ResumeExperience id="experience"></ResumeExperience>
    <ResumePortfolio id="portfolio"></ResumePortfolio>
</template>

<style scoped>

</style>
