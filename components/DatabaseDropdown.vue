<template>
  <b-dropdown class="dropdown" variant="link" no-caret>
    <template #button-content>
      <img src="/database_icon.png" alt="Database Icon" class="category-icon"/>
      <span class="dropdown-text">Database</span>
    </template>
    <b-dropdown-item to="/database/characters">
      <img src="/Mayreel_5.png" alt="Character Icon" class="dropdown-icon"/>
      Characters
    </b-dropdown-item>
    <b-dropdown-item to="/database/weapons">
      <img src="/weapons_icon.png" alt="Weapons Icon" class="dropdown-icon"/>
      Weapons
    </b-dropdown-item>
    <!-- ...other database categories -->
  </b-dropdown>
</template>

  
  <style scoped>
  .category-icon,
  .dropdown-icon {
    width: 20px;
    height: auto;
    margin-right: 5px;
  }
  </style>
  