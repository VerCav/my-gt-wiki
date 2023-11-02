<template>
  <div class="banner">
    <nuxt-link to="/">
      <img src="/GTlogo.png" alt="Guardian Tales Logo" class="logo" />
    </nuxt-link>
    <DatabaseDropdown />
    <GuidesDropdown />
    <ToolsDropdown />
    <LoreDropdown />
    <div class="nav-links">
      <nuxt-link to="/news">
        <img src="/news_icon.png" alt="News Icon" class="category-icon"/>
        News
      </nuxt-link>
      <nuxt-link to="/tier-list">
        <img src="/tier_list_icon.png" alt="Tier List Icon" class="category-icon"/>
        Tier List
      </nuxt-link>
    </div>
    <div class="icons">
      <button class="search-icon">🔍</button>
      <button class="user-icon">👤</button>
    </div>
  </div>
</template>

<script>
import DatabaseDropdown from '~/components/DatabaseDropdown.vue'; 
import GuidesDropdown from '~/components/GuidesDropdown.vue';

export default {
  components: {
    DatabaseDropdown,
    GuidesDropdown,
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@700&display=swap');

.banner {
  background-color: #2f261c; /* light brown */
  background-size: cover;
  background-repeat: no-repeat;
  background: linear-gradient(#2d2523, #534d45);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  display: flex;
  align-items: center;
  padding: 1vh 1vw; /* Using viewport units */
  border-top: 2px solid white;
  border-bottom: 2px solid white;
  height: 10vh;
}

.logo {
  height: auto;
  width: auto;
  max-height: 10vh;  /* Using viewport units */
  padding: 1vh 1vw 1vh 2vw; /* top, right, bottom, left */
}

.nav-links {
  flex-grow: 1;
  text-align: center;
}

.nav-links a {
  color: #f3ede4; /* primary text color */
  font-family: 'Roboto', sans-serif;
  font-size: 1.5em;
}

.icons {
  margin-left: auto;
}

.search-icon,
.user-icon {
  background: none;
  border: none;
  font-size: 1.2em;
  cursor: pointer;
}
.button {
  border-radius: 12px;
  /* ...other styles */
}
.overlay {
  position: absolute;
  z-index: 1;
  /* ...other styles */
}
.character-icon {
  height: auto;
  width: auto;
  max-height: 2em;  /* Adjust size as needed */
  margin-right: 0em;  /* Space between image and text */
}
/* Remove default background and borders from dropdowns */
.dropdown {
  background: none;
  border: none;
  outline: none;
}

/* Style the dropdown text */
.dropdown-text {
  color: #f3ede4; /* primary text color from your banner */
  font-family: 'Roboto', sans-serif;
  font-size: 1.5em;
  text-decoration: none; /* Remove underlines */
}
.nav-links a, .dropdown {
  margin: 0 1em; /* Horizontal spacing */
}

.nav-links a:hover, .dropdown:hover {
  color: #dad075; /* A different color for hover state */
}

.nav-links a, .dropdown {
  font-weight: bold;
}
</style>