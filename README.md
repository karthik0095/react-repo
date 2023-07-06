# react-repo

<template>
  <nav class="sidebar">
    <ul class="nav flex-column">
      <li class="nav-item">
        <a class="nav-link" @click="toggleMenu('dataIngestion')">
          Data Ingestion
          <i class="fas fa-chevron-right float-right" :class="{ 'open': isMenuOpen('dataIngestion') }"></i>
        </a>
        <ul class="sub-menu" :class="{ 'show': isMenuOpen('dataIngestion') }">
          <li><router-link to="/data-ingestion/option1">Option 1</router-link></li>
          <li><router-link to="/data-ingestion/option2">Option 2</router-link></li>
          <li><router-link to="/data-ingestion/option3">Option 3</router-link></li>
        </ul>
      </li>
      <li class="nav-item">
        <a class="nav-link" @click="toggleMenu('configuration')">
          Configuration
          <i class="fas fa-chevron-right float-right" :class="{ 'open': isMenuOpen('configuration') }"></i>
        </a>
        <ul class="sub-menu" :class="{ 'show': isMenuOpen('configuration') }">
          <li><router-link to="/configuration/option1">Option 1</router-link></li>
          <li><router-link to="/configuration/option2">Option 2</router-link></li>
        </ul>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      openMenus: [],
    };
  },
  methods: {
    toggleMenu(menu) {
      if (this.isMenuOpen(menu)) {
        this.openMenus = this.openMenus.filter(item => item !== menu);
      } else {
        this.openMenus.push(menu);
      }
    },
    isMenuOpen(menu) {
      return this.openMenus.includes(menu);
    },
  },
};
</script
  <!DOCTYPE html>
<html lang="en">
<head>
  <!-- Other head elements -->
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome
  
