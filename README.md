<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Deluxe Tours & Travels</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="font-sans text-gray-800">
  <!-- Navbar -->
  <nav class="flex justify-between items-center p-5 shadow-md bg-white sticky top-0 z-50">
    <h1 class="text-2xl font-bold text-blue-600">Deluxe Tours & Travels</h1>
    <div class="space-x-5 hidden md:flex">
      <a href="#destinations" class="hover:text-blue-500">Destinations</a>
      <a href="#booking" class="hover:text-blue-500">Book Now</a>
      <a href="#testimonials" class="hover:text-blue-500">Testimonials</a>
      <a href="#about" class="hover:text-blue-500">About Us</a>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="min-h-[70vh] flex items-center justify-center text-white text-center"
    style="background-image: url('https://source.unsplash.com/1600x600/?travel,adventure'); background-size: cover; background-position: center;">
    <div>
      <h2 class="text-5xl font-bold mb-4 drop-shadow-lg">Explore the World with Us</h2>
      <p class="text-lg mb-6 drop-shadow">Your journey begins here</p>
      <a href="#booking" class="bg-blue-600 text-white px-6 py-3 rounded-full shadow-lg hover:bg-blue-700">Plan Your Trip</a>
    </div>
  </section>

  <!-- Destinations -->
  <section id="destinations" class="py-12 px-6 bg-gray-50">
    <h3 class="text-3xl font-bold text-center mb-8">Popular Destinations</h3>
    <div class="grid sm:grid-cols-2 md:grid-cols-4 gap-6">
      <div class="shadow-lg rounded-2xl overflow-hidden bg-white">
        <img src="https://source.unsplash.com/600x400/?paris,travel" alt="Paris" class="h-48 w-full object-cover" />
        <div class="p-4 text-center font-semibold">Paris</div>
      </div>
      <div class="shadow-lg rounded-2xl overflow-hidden bg-white">
        <img src="https://source.unsplash.com/600x400/?bali,beach" alt="Bali" class="h-48 w-full object-cover" />
        <div class="p-4 text-center font-semibold">Bali</div>
      </div>
      <div class="shadow-lg rounded-2xl overflow-hidden bg-white">
        <img src="https://source.unsplash.com/600x400/?newyork,city" alt="New York" class="h-48 w-full object-cover" />
        <div class="p-4 text-center font-semibold">New York</div>
      </div>
      <div class="shadow-lg rounded-2xl overflow-hidden bg-white">
        <img src="https://source.unsplash.com/600x400/?switzerland,mountains" alt="Switzerland" class="h-48 w-full object-cover" />
        <div class="p-4 text-center font-semibold">Switzerland</div>
      </div>
    </div>
  </section>

  <!-- Booking Form -->
  <section id="booking" class="py-12 px-6">
    <h3 class="text-3xl font-bold text-center mb-8">Book Your Trip</h3>
    <form onsubmit="handleSubmit(event)" class="max-w-xl mx-auto bg-white p-8 shadow-lg rounded-2xl space-y-4">
      <input type="text" id="name" placeholder="Full Name" required class="w-full border p-3 rounded" />
      <input type="email" id="email" placeholder="Email" required class="w-full border p-3 rounded" />
      <input type="text" id="destination" placeholder="Preferred Destination" required class="w-full border p-3 rounded" />
      <input type="date" id="date" required class="w-full border p-3 rounded" />
      <button type="submit" class="w-full bg-blue-600 text-white py-3 rounded-lg hover:bg-blue-700">Submit</button>
    </form>
  </section>

  <!-- Testimonials -->
  <section id="testimonials" class="py-12 px-6 bg-gray-50">
    <h3 class="text-3xl font-bold text-center mb-8">What Our Customers Say</h3>
    <div class="grid md:grid-cols-3 gap-6">
      <div class="p-6 shadow-md rounded-2xl text-center bg-white">
        <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Sarah Johnson" class="w-16 h-16 rounded-full mx-auto mb-4" />
        <p class="italic mb-4">“The trip was perfectly organized, had the best experience!”</p>
        <h4 class="font-semibold">- Sarah Johnson</h4>
      </div>
      <div class="p-6 shadow-md rounded-2xl text-center bg-white">
        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Michael Lee" class="w-16 h-16 rounded-full mx-auto mb-4" />
        <p class="italic mb-4">“Amazing service and unforgettable destinations.”</p>
        <h4 class="font-semibold">- Michael Lee</h4>
      </div>
      <div class="p-6 shadow-md rounded-2xl text-center bg-white">
        <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Priya Sharma" class="w-16 h-16 rounded-full mx-auto mb-4" />
        <p class="italic mb-4">“Deluxe Tours made our honeymoon truly magical!”</p>
        <h4 class="font-semibold">- Priya Sharma</h4>
      </div>
    </div>
  </section>

  <!-- About Us -->
  <section id="about" class="py-12 px-6">
    <h3 class="text-3xl font-bold text-center mb-8">About Us</h3>
    <div class="max-w-3xl mx-auto text-center text-lg leading-relaxed">
      <p>
        Deluxe Tours and Travels is your trusted partner in exploring the world. With years of experience in crafting unforgettable journeys, we specialize in personalized travel packages that cater to every traveler’s dream. Whether it’s a romantic getaway, a family vacation, or an adventurous trip, we ensure comfort, quality, and lasting memories.
      </p>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-blue-600 text-white py-6 text-center">
    <p>© <span id="year"></span> Deluxe Tours & Travels. All rights reserved.</p>
  </footer>

  <script>
    document.getElementById("year").textContent = new Date().getFullYear();
    function handleSubmit(event) {
      event.preventDefault();
      alert("Booking submitted! We'll contact you soon.");
      document.querySelector("form").reset();
    }
  </script>
</body>
</html>
