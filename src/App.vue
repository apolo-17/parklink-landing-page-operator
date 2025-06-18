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
      <div class="space-x-4">
        <a
          href="https://parklinkapp.laravel.cloud/register?role=operator"
          class="inline-block rounded-xl bg-white px-6 py-3 font-semibold text-blue-700 hover:bg-gray-100"
        >
          Soy operador
        </a>
        <a
          href="#"
          class="inline-block rounded-xl bg-blue-500 px-6 py-3 font-semibold text-white hover:bg-blue-600"
        >
          Soy conductor
        </a>
      </div>
    </section>

    <!-- Beneficios para operadores -->
    <section id="features-operators" class="bg-gray-100 py-16">
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
              <circle cx="12" cy="12" r="10" />
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
              <rect x="3" y="3" width="7" height="7" rx="1" ry="1" />
              <rect x="14" y="3" width="7" height="7" rx="1" ry="1" />
              <rect x="3" y="14" width="7" height="7" rx="1" ry="1" />
              <rect x="14" y="14" width="7" height="7" rx="1" ry="1" />
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
              <circle cx="12" cy="12" r="10" />
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

    <!-- Beneficios para conductores -->
    <section id="features-drivers" class="bg-white py-16">
      <div class="container mx-auto px-4 text-center">
        <h3 class="mb-8 text-2xl font-bold">Beneficios para conductores</h3>
        <div class="grid gap-8 md:grid-cols-4">
          <div>
            <svg
              class="mx-auto mb-4 h-12 w-12 text-blue-500"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path d="M3 10h11v4H3z" />
              <path d="M18 6h3v12h-3" />
            </svg>
            <h4 class="text-lg font-semibold">Escaneo rápido</h4>
            <p>Entra y sal con solo escanear un código QR.</p>
          </div>
          <div>
            <svg
              class="mx-auto mb-4 h-12 w-12 text-blue-500"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path d="M4 6h16M4 12h8m-8 6h16" />
            </svg>
            <h4 class="text-lg font-semibold">Pago desde el celular</h4>
            <p>Olvídate del efectivo, paga fácil desde tu teléfono.</p>
          </div>
          <div>
            <svg
              class="mx-auto mb-4 h-12 w-12 text-blue-500"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path d="M8 7h8v10H8z" />
              <path d="M6 3h12v18H6z" />
            </svg>
            <h4 class="text-lg font-semibold">Boleto digital</h4>
            <p>Accede a tu ticket desde cualquier dispositivo.</p>
          </div>
          <div>
            <svg
              class="mx-auto mb-4 h-12 w-12 text-blue-500"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
            >
              <path d="M5 12h14M12 5l7 7-7 7" />
            </svg>
            <h4 class="text-lg font-semibold">Historial completo</h4>
            <p>Consulta tus entradas y pagos anteriores.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- (contenido existente conservado) -->
    <section id="how-it-works" class="bg-gray-100 py-16">
      <div class="container mx-auto px-4 text-center">
        <h3 class="mb-8 text-2xl font-bold">¿Cómo funciona?</h3>
        <div class="grid md:grid-cols-2 gap-8 items-center">
          <div>
            <img
              src="https://placehold.co/600x400?text=Mapa+QR"
              alt="Vista del sistema"
              class="mx-auto rounded-lg shadow-md"
            />
          </div>
          <div class="text-left">
            <ol class="list-decimal list-inside space-y-4">
              <li>El conductor escanea un QR al entrar al estacionamiento.</li>
              <li>
                El sistema registra la entrada y genera un boleto digital.
              </li>
              <li>
                Al salir, el sistema calcula el tiempo y muestra el monto.
              </li>
              <li>El conductor paga desde su celular y se abre la salida.</li>
            </ol>
          </div>
        </div>
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

    <!-- Contact Email -->
    <section class="bg-gray-100 py-12 text-center">
      <div class="container mx-auto px-4">
        <h3 class="mb-4 text-2xl font-bold text-gray-800">
          ¿Tienes dudas o quieres colaborar?
        </h3>
        <p class="text-lg text-gray-700">
          Escríbenos a
          <a
            href="mailto:hola@parklink.com.mx"
            class="text-blue-600 hover:underline font-semibold"
          >
            hola@parklink.com.mx
          </a>
        </p>
      </div>
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
