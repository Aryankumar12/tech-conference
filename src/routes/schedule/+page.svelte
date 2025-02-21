<script>
    const schedule = [
      {
        date: "March 10, 2025",
        time: "10:00 AM - 11:00 AM",
        topic: "The Future of AI",
        speaker: "Jane Doe"
      },
      {
        date: "March 10, 2025",
        time: "11:30 AM - 12:30 PM",
        topic: "Innovating with Blockchain",
        speaker: "John Smith"
      },
      {
        date: "March 11, 2025",
        time: "09:00 AM - 10:00 AM",
        topic: "Cybersecurity in 2025",
        speaker: "Emily Johnson"
      },
      {
        date: "March 11, 2025",
        time: "1:00 PM - 2:00 PM",
        topic: "Building Scalable Web Apps",
        speaker: "Michael Brown"
      }
    ];
  </script>
  
  <!-- Schedule Section -->
  <section class="min-h-screen py-12 px-6 bg-gray-900 text-white">
    <h1 class="text-4xl font-bold text-center mb-12 text-indigo-400">Conference Schedule</h1>
  
    <!-- Schedule Table -->
    <div class="bg-gray-800 rounded-lg shadow-lg overflow-hidden">
      <table class="w-full text-left table-auto border-collapse">
        <thead>
          <tr class="bg-indigo-500 text-white">
            <th class="px-6 py-3 border-b">Date</th>
            <th class="px-6 py-3 border-b">Time</th>
            <th class="px-6 py-3 border-b">Topic</th>
            <th class="px-6 py-3 border-b">Speaker</th>
          </tr>
        </thead>
        <tbody>
          {#each schedule as session}
            <tr class="hover:bg-gray-700">
              <td class="px-6 py-4 border-b border-gray-700">{session.date}</td>
              <td class="px-6 py-4 border-b border-gray-700">{session.time}</td>
              <td class="px-6 py-4 border-b border-gray-700">{session.topic}</td>
              <td class="px-6 py-4 border-b border-gray-700">{session.speaker}</td>
            </tr>
          {/each}
        </tbody>
      </table>
    </div>
  </section>
  