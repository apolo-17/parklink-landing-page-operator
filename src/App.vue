<template>
  <div class="min-h-screen bg-white text-gray-800">
    <!-- Navbar (fixed) -->
    <header class="fixed top-0 z-50 w-full bg-white shadow">
      <div class="container mx-auto flex items-center justify-between p-4">
        <h1 class="text-3xl font-black text-blue-800">
          Park<span class="text-blue-500">Link</span>
        </h1>
        <button class="md:hidden">
          <svg
            class="h-6 w-6 text-blue-800"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            />
          </svg>
        </button>
        <nav class="hidden space-x-6 md:flex">
          <a href="#features" class="hover:text-blue-500">Beneficios</a>
          <a href="#how-it-works" class="hover:text-blue-500">Cómo Funciona</a>
          <a href="#testimonials" class="hover:text-blue-500">Testimonios</a>
          <a href="#partners" class="hover:text-blue-500">Socios</a>
          <a href="#contact" class="hover:text-blue-500">Contacto</a>
        </nav>
      </div>
    </header>

    <!-- Spacer for fixed header -->
    <div class="h-20"></div>

    <!-- Hero -->
    <section class="bg-blue-900 py-20 text-center text-white">
      <h2 class="mb-4 text-4xl font-bold md:text-5xl">
        Moderniza tu estacionamiento con ParkLink
      </h2>
      <p class="mb-8 text-lg md:text-xl">
        Digitaliza el cobro, mejora la experiencia del cliente y administra
        desde cualquier lugar.
      </p>
      <a
        href="https://parklinkapp.laravel.cloud/register?role=operator"
        class="inline-block rounded-xl bg-blue-500 px-6 py-3 font-semibold text-white hover:bg-blue-600"
        >Registrarse</a
      >
    </section>

    <!-- Features -->
    <section id="features" class="bg-gray-100 py-16">
      <div class="container mx-auto px-4 text-center">
        <h3 class="mb-8 text-2xl font-bold">Beneficios para operadores</h3>
        <div class="grid gap-8 md:grid-cols-3">
          <div>
            <svg
              class="mx-auto mb-4 h-12 w-12 text-blue-500"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              viewBox="0 0 24 24"
            >
              <circle
                cx="12"
                cy="12"
                r="10"
                stroke="currentColor"
                stroke-width="2"
                fill="none"
              />
              <path
                d="M12 6v6l3 3"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <h4 class="text-lg font-semibold">Cobros automatizados</h4>
            <p>
              Recibe pagos directo a tu cuenta bancaria con integración a
              Stripe.
            </p>
          </div>
          <div>
            <svg
              class="mx-auto mb-4 h-12 w-12 text-blue-500"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              viewBox="0 0 24 24"
            >
              <rect
                x="3"
                y="3"
                width="7"
                height="7"
                rx="1"
                ry="1"
                stroke="currentColor"
              />
              <rect
                x="14"
                y="3"
                width="7"
                height="7"
                rx="1"
                ry="1"
                stroke="currentColor"
              />
              <rect
                x="3"
                y="14"
                width="7"
                height="7"
                rx="1"
                ry="1"
                stroke="currentColor"
              />
              <rect
                x="14"
                y="14"
                width="7"
                height="7"
                rx="1"
                ry="1"
                stroke="currentColor"
              />
            </svg>
            <h4 class="text-lg font-semibold">Control total</h4>
            <p>
              Administra tus tickets, staff y reportes desde cualquier
              dispositivo.
            </p>
          </div>
          <div>
            <svg
              class="mx-auto mb-4 h-12 w-12 text-blue-500"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              viewBox="0 0 24 24"
            >
              <circle cx="12" cy="12" r="10" stroke="currentColor" />
              <path
                d="M9 12l2 2 4-4"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <h4 class="text-lg font-semibold">Fácil de usar</h4>
            <p>
              Tu personal se adapta rápido sin capacitación compleja ni hardware
              especial.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Cómo aparecen en el mapa -->
    <section class="px-4 py-16 text-center">
      <div class="mx-auto max-w-3xl">
        <h3 class="mb-4 text-2xl font-bold">
          Tus estacionamientos visibles al mundo
        </h3>
        <p class="mb-4">
          Cada estacionamiento registrado será visible en nuestra plataforma web
          y en mapas como Google Maps. Los usuarios podrán calificar, recomendar
          y encontrar tu ubicación en línea.
        </p>
        <p>
          Trabajamos con plataformas como Google Maps, Waze y próximamente otras
          apps de movilidad para mostrar tu negocio donde tus clientes están
          buscando.
        </p>
      </div>
    </section>

    <!-- Testimonials -->
    <section id="testimonials" class="bg-gray-100 py-16">
      <div class="container mx-auto px-4 text-center">
        <h3 class="mb-8 text-2xl font-bold">Lo que dicen nuestros clientes</h3>
        <div class="grid gap-8 md:grid-cols-3">
          <div class="rounded-xl bg-white p-6 shadow">
            <img
              src="https://randomuser.me/api/portraits/men/32.jpg"
              alt="Juan Pérez"
              class="mx-auto mb-4 h-16 w-16 rounded-full"
            />
            <p class="italic">
              “Desde que usamos ParkLink, todo es más ágil. Los clientes pagan
              sin bajarse del auto.”
            </p>
            <div class="my-2 text-yellow-400">★★★★★</div>
            <p class="mt-2 font-bold">Juan Pérez, Estacionamiento Centro</p>
          </div>
          <div class="rounded-xl bg-white p-6 shadow">
            <img
              src="https://randomuser.me/api/portraits/women/44.jpg"
              alt="Laura Méndez"
              class="mx-auto mb-4 h-16 w-16 rounded-full"
            />
            <p class="italic">
              “La app es intuitiva, mis empleados aprendieron a usarla en un
              solo día.”
            </p>
            <div class="my-2 text-yellow-400">★★★★☆</div>
            <p class="mt-2 font-bold">Laura Méndez, AutoPark Sur</p>
          </div>
          <div class="rounded-xl bg-white p-6 shadow">
            <img
              src="https://randomuser.me/api/portraits/men/75.jpg"
              alt="Carlos Ramírez"
              class="mx-auto mb-4 h-16 w-16 rounded-full"
            />
            <p class="italic">
              “Puedo ver mis ingresos diarios desde mi celular. ¡Lo recomiendo!”
            </p>
            <div class="my-2 text-yellow-400">★★★★★</div>
            <p class="mt-2 font-bold">Carlos Ramírez, Parking Norte</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Partners Carousel -->
    <section id="partners" class="bg-white py-16 text-center">
      <h3 class="mb-8 text-2xl font-bold">Nuestros socios y aliados</h3>
      <div
        class="relative flex flex-wrap justify-center gap-x-16 gap-y-12 px-6"
        style="min-height: 160px"
      >
        <!-- Google Maps -->
        <img
          src="https://cdn.worldvectorlogo.com/logos/google-maps-2020-icon.svg"
          alt="Google Maps"
          class="animate-flicker1 h-24 w-24 object-contain"
          style="transform: translateY(-10px)"
        />

        <!-- Waze -->
        <img
          src="https://static.cdnlogo.com/logos/w/7/waze.svg"
          alt="Waze"
          class="animate-flicker2 h-28 w-28 object-contain"
          style="transform: translateY(20px)"
        />

        <!-- Stripe -->
        <img
          src="https://cdn.worldvectorlogo.com/logos/stripe-4.svg"
          alt="Stripe"
          class="animate-flicker3 h-24 w-24 object-contain"
          style="transform: translateY(-5px)"
        />
      </div>
    </section>

    <!-- Contact CTA -->
    <section id="contact" class="bg-blue-700 py-20 text-center text-white">
      <h3 class="mb-4 text-3xl font-bold">
        ¡Transforma tu estacionamiento hoy!
      </h3>
      <p class="mb-6">Empieza gratis y lleva tu negocio al siguiente nivel.</p>
      <a
        href="https://parklinkapp.laravel.cloud/register?role=operator"
        class="inline-block rounded-xl bg-white px-6 py-3 font-semibold text-blue-700 hover:bg-gray-100"
        >Registrate ahora!</a
      >
    </section>

    <!-- Footer -->
    <footer class="bg-blue-900 py-4 text-center text-white">
      <p class="text-sm">
        &copy; 2025 ParkLink. Todos los derechos reservados.
      </p>
    </footer>
  </div>
</template>

<script setup>
// No se necesita JS por ahora
</script>

<style scoped>
@keyframes flicker {
  0%,
  100% {
    opacity: 1;
  }
  50% {
    opacity: 0.5;
  }
}

.animate-flicker1 {
  animation: flicker 2.8s infinite ease-in-out;
}

.animate-flicker2 {
  animation: flicker 3.6s infinite ease-in-out;
}

.animate-flicker3 {
  animation: flicker 4.2s infinite ease-in-out;
}
</style>
