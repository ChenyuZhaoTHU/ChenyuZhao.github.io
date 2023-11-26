<script setup>
import Bio from './components/Bio.vue'
import NewsList from './components/NewsList.vue'
import EducationList from './components/EducationList.vue'
import PublicationList from './components/PublicationList.vue'
import AwardList from './components/AwardList.vue'
import Footer from './components/Footer.vue'
import ProjectList from './components/ProjectList.vue'
</script>

<template>
  <header>
    <Bio />
    <hr>
  </header>

  <main>
    <NewsList />
    <hr>
    <EducationList />
    <hr>
    <PublicationList />
    <hr>
    <ProjectList />
    <hr>
    <AwardList />
    <hr>
    <!-- <TalkList /> -->
    <!-- <SoftwareList /> -->
    
  </main>

  <footer>
    <div class="row items-align-top">
      <div class="col" style="text-align: center; margin: auto;">
        <b>Relevant Links: </b>
        <a href="https://www.sigs.tsinghua.edu.cn/main.htm" target="_blank">Tsinghua University SIGS</a>
        | <a href="https://scholar.google.com.hk/citations?hl=zh-CN&user=Ha8rlUgAAAAJ&view_op=list_works&sortby=pubdate" target="_blank">Prof. Xinlei Chen</a>
        | <a href="https://www.csu.edu.cn/" target="_blank">Central South University</a>
        <br><br>Updated by Haoyang Wang in November 2023. 😜
      </div>
  </div>
  </footer>
</template>

<style>

</style>
