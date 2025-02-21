<script>
    const speakers = [
      {
        name: "Jane Doe",
        title: "CTO at TechCorp",
        bio: "An innovator in AI and machine learning with over a decade of experience in tech leadership.",
        image: "/images/men.jpeg"
      },
      {
        name: "John Smith",
        title: "CEO at Innovate Inc.",
        bio: "A visionary entrepreneur revolutionizing the world of technology with groundbreaking ideas.",
        image: "/images/men.jpeg"
      },
      {
        name: "Emily Johnson",
        title: "Head of AI at FutureTech",
        bio: "An expert in artificial intelligence and a passionate advocate for ethical AI.",
        image: "/images/men.jpeg"
      },
      {
        name: "Michael Brown",
        title: "Founder at DevSolutions",
        bio: "A software engineer turned founder, inspiring developers worldwide with his insights.",
        image: "/images/men.jpeg"
      }
    ];
  </script>
  
  <!-- Speakers Section -->
  <section class="min-h-screen flex flex-col items-center justify-center py-12 px-6 bg-gray-900 text-white">
    <h1 class="text-4xl font-bold text-center mb-8 text-indigo-400">Meet the Speakers</h1>
  
    <!-- Speaker Grid -->
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-8">
      {#each speakers as speaker}
        <div class="bg-gray-800 rounded-lg shadow-lg p-6 text-center">
          <img
            src={speaker.image}
            alt={speaker.name}
            class="w-32 h-32 rounded-full mx-auto mb-4 border-4 border-indigo-400"
          />
          <h2 class="text-xl font-bold text-indigo-300">{speaker.name}</h2>
          <p class="text-gray-400">{speaker.title}</p>
          <p class="text-gray-300 mt-4">{speaker.bio}</p>
        </div>
      {/each}
    </div>
  </section>
  