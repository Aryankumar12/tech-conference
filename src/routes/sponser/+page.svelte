<script>
    const sponsors = [
      { name: "TechCorp", logo: "/images/company.jpg", link: "https://www.techcorp.com" },
      { name: "Innovate Inc.", logo: "/images/company.jpg", link: "https://www.innovateinc.com" },
      { name: "FutureTech", logo: "/images/company.jpg", link: "https://www.futuretech.com" }
    ];
  </script>
  
  <section class="min-h-screen py-12 px-6 bg-gray-900 text-white">
    <h1 class="text-4xl font-bold text-center mb-8 text-indigo-400">Our Sponsors</h1>
    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
      {#each sponsors as sponsor}
        <a href={sponsor.link} target="_blank" class="bg-gray-800 rounded-lg shadow-lg p-6 text-center hover:shadow-2xl">
          <img
            src={sponsor.logo}
            alt={sponsor.name}
            class="w-32 h-32 mx-auto mb-4 object-contain"
          />
          <h2 class="text-xl font-bold text-indigo-300">{sponsor.name}</h2>
        </a>
      {/each}
    </div>
  </section>
  