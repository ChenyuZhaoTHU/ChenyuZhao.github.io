<script setup>
import { computed } from 'vue'

import {convertNestedMarkdownContentToHtml} from '../utils'

import RecruitmentJson from '../content/recruitment.json'


const RecruitmentArr = computed(() => {
  return convertNestedMarkdownContentToHtml(RecruitmentJson)
})
const idPrefix = "Recruitment"

</script>

<template>
  <h2>Recruitment</h2>

  <!-- <div v-for="(projectList, listIdx) in RecruitmentArr" :key="listIdx"></div>
    <ul reversed>
      <li v-for="(project, index) in projectList.list" :key="index">
        <a style="font-size: 15pt" >{{ project.name }}</a><br>

        <div>

        </div>
      </li>
    </ul> -->

  <div v-for="(RecruitmentList, listIdx) in RecruitmentArr" :key="listIdx">
    <!-- <h3>{{ softwareList.category }}</h3> -->
    <div class="row items-align-top" v-for="(Recruitment, index) in RecruitmentList.list" :key="index">
      
      <p  v-html="Recruitment.content"></p>

      <!-- <div class="col flex-start tight-list" :id="`${idPrefix}-${listIdx}-${index}`" v-html="project.content"></div>
       -->
    </div>

  </div>




</template>