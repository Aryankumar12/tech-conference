<script>
    let name = "";
    let email = "";
    let message = "";
  
    function handleSubmit() {
      alert(`Thank you, ${name}! We will get back to you soon.`);
    }
  </script>
  
  <section class="min-h-screen py-12 px-6 bg-gray-900 text-white">
    <h1 class="text-4xl font-bold text-center mb-8 text-indigo-400">Contact Us</h1>
  
    <!-- Contact Form -->
    <form on:submit|preventDefault={handleSubmit} class="max-w-3xl mx-auto bg-gray-800 rounded-lg shadow-lg p-8">
      <div class="mb-6">
        <label for="name" class="block text-sm font-medium text-gray-400">Name</label>
        <input
          id="name"
          type="text"
          bind:value={name}
          class="w-full p-3 rounded-lg bg-gray-900 text-white border border-gray-700"
          placeholder="Your Name"
          required
        />
      </div>
  
      <div class="mb-6">
        <label for="email" class="block text-sm font-medium text-gray-400">Email</label>
        <input
          id="email"
          type="email"
          bind:value={email}
          class="w-full p-3 rounded-lg bg-gray-900 text-white border border-gray-700"
          placeholder="Your Email"
          required
        />
      </div>
  
      <div class="mb-6">
        <label for="message" class="block text-sm font-medium text-gray-400">Message</label>
        <textarea
          id="message"
          bind:value={message}
          class="w-full p-3 rounded-lg bg-gray-900 text-white border border-gray-700"
          placeholder="Your Message"
          rows="4"
          required
        ></textarea>
      </div>
  
      <button
        type="submit"
        class="w-full py-3 px-6 rounded-lg bg-indigo-500 text-white font-bold hover:bg-indigo-600"
      >
        Send Message
      </button>
    </form>
  
    <!-- Social Media Links -->
    <div class="text-center mt-8">
      <p class="text-gray-400">Follow us on social media:</p>
      <div class="flex justify-center space-x-6 mt-4">
        <a href="#" class="text-indigo-400 hover:text-white">Facebook</a>
        <a href="#" class="text-indigo-400 hover:text-white">Twitter</a>
        <a href="#" class="text-indigo-400 hover:text-white">LinkedIn</a>
      </div>
    </div>
  </section>
  