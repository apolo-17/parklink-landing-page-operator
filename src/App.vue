<template>
  <div class="min-h-screen bg-white text-gray-800">
    <!-- Navbar (fixed) -->
    <header class="fixed top-0 z-50 w-full bg-white shadow">
      <div class="container mx-auto flex items-center justify-between p-4">
        <h1 class="text-3xl font-black text-blue-800">
          Park<span class="text-blue-500">Link</span>
        </h1>

        <!-- Botón hamburguesa en mobile -->
        <button
          class="md:hidden"
          @click="toggleMenu"
          aria-label="Toggle navigation"
        >
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

        <!-- Menú desktop -->
        <nav class="hidden space-x-6 md:flex">
          <a href="#features" class="hover:text-blue-500">Beneficios</a>
          <a href="#how-it-works" class="hover:text-blue-500">Cómo Funciona</a>
          <a href="#testimonials" class="hover:text-blue-500">Testimonios</a>
          <a href="#partners" class="hover:text-blue-500">Socios</a>
          <a href="#contact" class="hover:text-blue-500">Contacto</a>
        </nav>
      </div>

      <!-- Menú mobile desplegable -->
      <div
        v-if="isMenuOpen"
        class="md:hidden bg-white shadow-inner px-4 pb-4 space-y-2"
      >
        <a href="#features" class="block text-blue-800 hover:text-blue-500"
          >Beneficios</a
        >
        <a href="#how-it-works" class="block text-blue-800 hover:text-blue-500"
          >Cómo Funciona</a
        >
        <a href="#testimonials" class="block text-blue-800 hover:text-blue-500"
          >Testimonios</a
        >
        <a href="#partners" class="block text-blue-800 hover:text-blue-500"
          >Socios</a
        >
        <a href="#contact" class="block text-blue-800 hover:text-blue-500"
          >Contacto</a
        >
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
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
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
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
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
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
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
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
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
        <div class="grid md:grid-cols-2 gap-12 items-center">
          <div>
            <img
              src="/map_lp_parklink_v2.png"
              alt="Vista del sistema"
              class="mx-auto w-full max-w-xl rounded-lg shadow-md"
            />
          </div>

          <!-- Instrucciones con íconos -->
          <div class="text-left space-y-6 md:pl-12">
            <!-- Paso 1 -->
            <div class="flex items-center space-x-4">
              <svg
                class="h-10 w-10 text-blue-500"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                viewBox="0 0 24 24"
              >
                <path d="M3 10h11v4H3z" />
                <path d="M18 6h3v12h-3" />
              </svg>
              <p class="text-lg">
                El conductor escanea un QR al entrar al estacionamiento.
              </p>
            </div>

            <!-- Paso 2 -->
            <div class="flex items-center space-x-4">
              <svg
                class="h-10 w-10 text-blue-500"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                viewBox="0 0 24 24"
              >
                <path d="M4 6h16M4 12h8m-8 6h16" />
              </svg>
              <p class="text-lg">
                El sistema registra la entrada y genera un boleto digital.
              </p>
            </div>

            <!-- Paso 3 -->
            <div class="flex items-center space-x-4">
              <svg
                class="h-10 w-10 text-blue-500"
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
              <p class="text-lg">
                Al salir, el sistema calcula el tiempo y muestra el monto.
              </p>
            </div>

            <!-- Paso 4 -->
            <div class="flex items-center space-x-4">
              <svg
                class="h-10 w-10 text-blue-500"
                fill="none"
                stroke="currentColor"
                stroke-width="2"
                viewBox="0 0 24 24"
              >
                <path d="M5 12h14M12 5l7 7-7 7" />
              </svg>
              <p class="text-lg">
                El conductor paga desde su celular y se abre la salida.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Testimonials (Carrusel continuo) -->
    <!-- Testimonials (Carrusel continuo con degradado azul) -->
    <section
      id="testimonials"
      class="bg-gradient-to-r from-blue-50 to-blue-100 py-16 overflow-hidden"
      @mouseenter="isPaused = true"
      @mouseleave="isPaused = false"
    >
      <div class="container mx-auto px-4 text-center">
        <h3 class="mb-8 text-2xl font-bold text-gray-800">
          Lo que dicen nuestros clientes
        </h3>

        <div
          ref="carouselRef"
          class="flex gap-6 w-full overflow-x-auto scroll-smooth"
          style="scrollbar-width: none; -ms-overflow-style: none"
        >
          <!-- Duplicamos testimonios para scroll infinito visual -->
          <template
            v-for="(testimonial, index) in [...testimonials, ...testimonials]"
            :key="index"
          >
            <div
              class="min-w-[300px] max-w-xs flex-shrink-0 rounded-xl bg-white p-6 shadow text-left"
            >
              <img
                :src="testimonial.image"
                :alt="testimonial.name"
                class="mb-4 h-16 w-16 rounded-full mx-auto"
              />
              <p class="italic text-sm md:text-base text-gray-700">
                “{{ testimonial.comment }}”
              </p>
              <div class="my-2 text-yellow-400 text-center">
                {{ testimonial.stars }}
              </div>
              <p
                class="mt-2 font-bold text-sm md:text-base text-center text-gray-800"
              >
                {{ testimonial.name }}, {{ testimonial.role }}
              </p>
            </div>
          </template>
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
import { ref, onMounted, onUnmounted } from "vue";

// Lógica del menú responsive
const isMenuOpen = ref(false);
const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};

// Lógica del carrusel continuo horizontal
const isPaused = ref(false);
const carouselRef = ref(null);
const speed = 0.5; // Ajusta la velocidad del scroll
let animationFrame;

const scrollCarousel = () => {
  if (!isPaused.value && carouselRef.value) {
    carouselRef.value.scrollLeft += speed;
    // Reinicio suave al final
    if (carouselRef.value.scrollLeft >= carouselRef.value.scrollWidth / 2) {
      carouselRef.value.scrollLeft = 0;
    }
  }
  animationFrame = requestAnimationFrame(scrollCarousel);
};

onMounted(() => {
  animationFrame = requestAnimationFrame(scrollCarousel);
});

onUnmounted(() => {
  cancelAnimationFrame(animationFrame);
});

// Lista de testimonios (repetidos para scroll continuo)
const testimonials = [
  {
    name: "Juan Pérez",
    role: "Estacionamiento Centro",
    comment:
      "Desde que usamos ParkLink, todo es más ágil. Los clientes pagan sin bajarse del auto.",
    stars: "★★★★★",
    image: "https://randomuser.me/api/portraits/men/32.jpg",
  },
  {
    name: "Laura Méndez",
    role: "AutoPark Sur",
    comment:
      "La app es intuitiva, mis empleados aprendieron a usarla en un solo día.",
    stars: "★★★★☆",
    image: "https://randomuser.me/api/portraits/women/44.jpg",
  },
  {
    name: "Carlos Ramírez",
    role: "Parking Norte",
    comment: "Puedo ver mis ingresos diarios desde mi celular. ¡Lo recomiendo!",
    stars: "★★★★★",
    image: "https://randomuser.me/api/portraits/men/75.jpg",
  },
  {
    name: "Andrea López",
    role: "Conductora frecuente",
    comment:
      "Me encanta no tener que buscar efectivo, todo es desde el celular.",
    stars: "★★★★★",
    image: "https://randomuser.me/api/portraits/women/65.jpg",
  },
  {
    name: "Eduardo Torres",
    role: "Conductor",
    comment:
      "Los boletos digitales me han salvado, ya no pierdo mis comprobantes.",
    stars: "★★★★★",
    image: "https://randomuser.me/api/portraits/men/51.jpg",
  },
  {
    name: "María Gómez",
    role: "Dueña de Parking San Pedro",
    comment:
      "Con ParkLink tengo control total de mis tickets. Ya no hay pérdidas.",
    stars: "★★★★★",
    image: "https://randomuser.me/api/portraits/women/20.jpg",
  },
];
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

@keyframes marquee {
  0% {
    transform: translateX(0%);
  }
  100% {
    transform: translateX(-50%);
  }
}

.animate-marquee {
  animation: marquee var(--animation-duration, 40s) linear infinite;
}
</style>
