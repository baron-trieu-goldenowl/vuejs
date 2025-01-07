<template>
  <div class="min-h-screen bg-white">
    <!-- Header -->
    <header class="container mx-auto px-4 py-4 flex items-center justify-between animate-fade-in">
      <div class="flex items-center gap-12">
        <img src="https://via.placeholder.com/800x400?text=ShopDemo" alt="Ella Logo" class="h-10" />
      </div>
    </header>

    <!-- Hero Section -->
    <main class="container mx-auto px-4 py-20 flex flex-col md:flex-row items-center gap-12">
      <!-- Left Content -->
      <div class="flex-1 animate-slide-up">
        <h1 class="text-5xl font-bold mb-6">
          Canva
          <br />
          multi-purpose
          <br />
          <span class="text-orange-500">Shopify</span>
        </h1>

        <div class="mb-6">
          <span class="text-orange-500 font-semibold">Shopify is the Best Selling</span>
          <span class="text-gray-700"> Shopify Theme of all time on Envato.</span>
        </div>

        <p class="text-gray-600 mb-8">
          An all-in-one template for your Shopify store, allowing you to create various structures and meet specific requirements.
        </p>
      </div>

      <!-- Right Content - Device Mockups -->
      <div class="flex-1 relative animate-float">
        <div class="relative">
          <img
            src="https://via.placeholder.com/800x400?text=ShopDemo"
            alt="Theme Preview"
            class="w-full rounded-lg shadow-2xl"
          />
          <div class="absolute -bottom-10 -right-10 bg-white p-4 rounded-lg shadow-lg animate-bounce-slow">
            <span class="text-sm font-medium">Discover now ! ⭐</span>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const menuItems = [
  'Home',
  'Page Layouts',
  'Features',
  'Performance',
  'User Guide',
  'Help'
]
</script>

<style scoped>
.animate-slide-down {
  animation: slideDown 0.5s ease-out;
}

.animate-slide-up {
  animation: slideUp 0.8s ease-out;
}

.animate-fade-in {
  animation: fadeIn 1s ease-out;
}

.animate-float {
  animation: float 3s ease-in-out infinite;
}

.animate-bounce-slow {
  animation: bounceSlow 2s ease-in-out infinite;
}

@keyframes slideDown {
  from {
    transform: translateY(-100%);
    opacity: 0;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}

@keyframes slideUp {
  from {
    transform: translateY(50px);
    opacity: 0;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@keyframes float {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-20px);
  }
}

@keyframes bounceSlow {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
}
</style>
