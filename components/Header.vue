<template>
  <header class="flex items-center flex-wrap">
    <div style="height: 54px" class="pr-5">
      <img src="/assets/images/gear.png" alt="logo" class="h-full" />
    </div>
    <div class="dropdown-menu">
      <button @click="toggleDropdown" class="dropdown-toggle">
        <svg
          class="w-6 h-6 text-white hover:text-teal-500 cursor-pointer"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16m-7 6h7"
          />
        </svg>
      </button>
      <div :class="{ 'dropdown-content': isDropdownOpen }">
        <ul class="flex flex-col items-center sm:flex-row sm:items-center">
          <li>
            <NuxtLink
              class="text-white hover:text-teal-500 text-lg px-4 py-3"
              to="/"
            >
              Home
            </NuxtLink>
          </li>
          <li>
            <a class="text-white hover:text-teal-500 text-lg px-4 py-3" href="#"
              >Popular</a
            >
          </li>
          <li>
            <a class="text-white hover:text-teal-500 text-lg px-4 py-3" href="#"
              >Features</a
            >
          </li>
          <li>
            <a class="text-white hover:text-teal-500 text-lg px-4 py-3" href="#"
              >Newcomers</a
            >
          </li>
        </ul>
      </div>
    </div>
    <ul class="flex ml-auto items-center mt-2">
      <li>
        <NuxtLink
          to="/register"
          class="inline-block bg-transparent border-white border hover:bg-white hover:bg-opacity-25 text-white font-light w-40 text-center px-6 py-1 text-lg rounded-full mr-4"
        >
          Sign Up
        </NuxtLink>
      </li>
      <li>
        <NuxtLink
          to="/login"
          class="inline-block bg-transparent border-white border hover:bg-white hover:bg-opacity-25 text-white font-light w-40 text-center px-6 py-1 text-lg rounded-full"
        >
          My Account
        </NuxtLink>
      </li>
      <!-- Add dark mode toggle button -->
      <li>
        <button @click="toggleDarkMode" class="dark-mode-toggle focus:outline-none">
          <svg
            class="w-6 h-6 text-white fill-current"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
          >
            <path
              v-if="!isDarkMode"
              d="M2.5 2.5v19h19v-19h-19zm3 3h13v13h-13v-13z"
            />
            <path
              v-else
              d="M13 2.5v13h-13v-13h13zm-13 16.5v-13h13v13h-13z"
            />
          </svg>
        </button>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isDropdownOpen: false,
      isDarkMode: false
    };
  },
  methods: {
    toggleDropdown() {
      this.isDropdownOpen = !this.isDropdownOpen;
    },
    toggleDarkMode() {
      this.isDarkMode = !this.isDarkMode;
      document.body.classList.toggle('dark-mode'); // Toggle dark mode class on body
    }
  }
};
</script>

<style scoped>
.dropdown-menu {
  position: relative;
}

.dropdown-toggle {
  background: transparent;
  border: none;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: #333;
  min-width: 260px;
  z-index: 1;
  box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
}

.dropdown-content a {
  color: white;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

.dropdown-content a:hover {
  background-color: #555;
}

.dropdown-content.show {
  display: block;
  .dark-mode .dropdown-content {
  background-color: #333;
}

.dark-mode .dropdown-content a {
  color: white;
}

.dark-mode .dropdown-content a:hover {
  background-color: #555;
}

.dark-mode .text-white {
  color: white;
}

.dark-mode .hover\:text-teal-500:hover {
  color: #4dc0b5;
}

.dark-mode .bg-transparent {
  background-color: transparent;
}

.dark-mode .hover\:bg-white:hover {
  background-color: white;
}

.dark-mode .border-white {
  border-color: white;
}

.dark-mode .hover\:bg-opacity-25:hover {
  background-color: rgba(255, 255, 255, 0.25);
}
}

@media (max-width: 768px) {
  .dropdown-toggle {
    display: flex;
    align-items: center;
  }
  .flex-col {
    flex-direction: column;
  }
}
</style>