<template>
  <header class="bg-white text-gray-800 border-b border-gray-200 shadow-sm p-4">
    <div class="container mx-auto flex">
      <div class="flex-shrink-0 mr-6">
        <!-- logo or brand name goes here -->
      </div>
      <div class="flex-grow flex items-center space-x-4">
        <!-- navigation links -->
        <a
          href="/"
          class="text-lg font-medium hover:text-blue-600 active:text-blue-800"
          >Home</a
        >
        <a
          href="/features"
          class="text-lg font-medium hover:text-blue-600 active:text-blue-800"
          >Features</a
        >
        <a
          href="/pricing"
          class="text-lg font-medium hover:text-blue-600 active:text-blue-800"
          >Pricing</a
        >
        <a
          href="/about"
          class="text-lg font-medium hover:text-blue-600 active:text-blue-800"
          >About</a
        >
      </div>
      <!-- search bar -->
      <div class="relative hidden sm:block ml-4">
        <input
          type="text"
          placeholder="Search..."
          class="border border-gray-300 rounded-md pl-10 pr-4 py-2 w-full focus:outline-none focus:ring focus:border-blue-300"
        />
        <span class="absolute top-0 left-0 mt-3 ml-3 inline-block">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            fill="currentColor"
            stroke="currentColor"
            class="h-6 w-6 text-gray-500"
          >
            <path
              d="M21 21l-5.2-5.2M10.5 18A7.5 7.5 0 1118 10.5 7.5 7.5 0 0110.5 18z"
            ></path>
          </svg>
        </span>
      </div>
    </div>
  </header>
</template>
