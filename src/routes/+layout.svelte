<script>
	let isMenuOpen = false; // To toggle the mobile menu
  </script>
  
  <header class="bg-gray-800 text-white py-4">
	<nav class="max-w-7xl mx-auto px-6 flex justify-between items-center">
	  <!-- Logo -->
	  <a href="/" class="text-xl font-bold text-indigo-400">Tech Conference 2025</a>
  
	  <!-- Desktop Menu -->
	  <div class="hidden md:flex space-x-4">
		<a href="/" class="hover:text-indigo-300">Home</a>
		<a href="/speaker" class="hover:text-indigo-300">Speakers</a>
		<a href="/schedule" class="hover:text-indigo-300">Schedule</a>
		<a href="/sponser" class="hover:text-indigo-300">Sponsors</a>
		<a href="/about" class="hover:text-indigo-300">About</a>
		<a href="/contact" class="hover:text-indigo-300">Contact</a>
	  </div>
  
	  <!-- Hamburger Icon for Mobile -->
	  <button
		class="md:hidden flex items-center focus:outline-none"
		on:click={() => (isMenuOpen = !isMenuOpen)}
	  >
		<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
		  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
		</svg>
	  </button>
	</nav>
  
	<!-- Mobile Menu -->
	{#if isMenuOpen}
	  <div class="md:hidden bg-gray-700 py-4">
		<a href="/" class="block px-6 py-2 hover:text-indigo-300">Home</a>
		<a href="/speaker" class="block px-6 py-2 hover:text-indigo-300">Speakers</a>
		<a href="/schedule" class="block px-6 py-2 hover:text-indigo-300">Schedule</a>
		<a href="/sponser" class="block px-6 py-2 hover:text-indigo-300">Sponsors</a>
		<a href="/about" class="block px-6 py-2 hover:text-indigo-300">About</a>
		<a href="/contact" class="block px-6 py-2 hover:text-indigo-300">Contact</a>
	  </div>
	{/if}
  </header>
  
  <!-- Page Content -->
  <main class="">
	<slot />
  </main>
  