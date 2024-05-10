<script setup>
import ApplicationLogo from "@/Components/ApplicationLogo.vue";
</script>

<template>
  <div>
    <button v-if="$page.props.user.permissions.includes('create roles')">
      Create Roles
    </button>
    <button v-if="$page.props.user.permissions.includes('create lessons')">
      Manage Lesson
    </button>
  </div>
</template>

<style>
button {
  background-color: #4caf50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  -webkit-transition-duration: 0.4s; /* Safari */
  transition-duration: 0.4s;
  cursor: pointer;
}
</style>
