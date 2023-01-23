<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'

const dateToday = new Date().toLocaleString();
const birthday = "HAPPY BIRTHDAY!!";
const birthdate = ''

function showDate (){
  return dateToday;
}

</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Today's Date is {{showDate()}}</template>
    <template #today></template>
  </WelcomeItem>
</template>
