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
    </ul>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isDropdownOpen: false
    };
  },
  methods: {
    toggleDropdown() {
      this.isDropdownOpen = !this.isDropdownOpen;
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