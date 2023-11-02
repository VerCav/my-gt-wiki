<template>
  <b-dropdown text="Guides" variant="info">
    <template #button-content>
      <img src="/Lahn_5.png" alt="Guides Icon" class="category-icon"/>
      Guides
    </template>
    <b-dropdown-item to="/guides/arena">
      <img src="/arena_icon.png" alt="Arena Icon" class="dropdown-icon"/>
      Arena
    </b-dropdown-item>
    <b-dropdown-item to="/guides/bosses">
      <img src="/bosses_icon.png" alt="Bosses Icon" class="dropdown-icon"/>
      Bosses
    </b-dropdown-item>
    <!-- ...other guide categories -->
  </b-dropdown>
</template>
