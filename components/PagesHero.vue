<template>
  <div>
    <header
      id="up"
      class="
        bg-center bg-fixed bg-no-repeat bg-center bg-cover
        h-screen
        relative
      "
    >
      <!-- Overlay Background + Center Control -->
      <div
        class="h-screen bg-opacity-50 bg-black flex items-center justify-center"
        style="background: rgba(0, 0, 0, 0.8)"
      >
        <div class="mx-2 text-center">
          <h1
            class="font-bold md:text-6xl text-5xl leading-tight text-white"
            style="font-family: 'Poppins', sans-serif"
          >
            {{ pageName }}
          </h1>
          <p class="text-xl pt-8 text-gray-100 pb-12 md:px-32">
            The Indian Society for Technical Education (ISTE) is the leading
            National Professional non-profit making Society for the Technical
            Education System in our country with the motto of Career Development
            of Teachers and Personality Development of Students and overall
            development of our Technical Education System.
          </p>
          <div class="inline-flex">
              <a href="#main">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="54"
                height="54"
                viewBox="0 0 24 24"
                fill="none"
                stroke="#ef4444"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
                class="feather scrollDown feather-arrow-down-circle animate__animated  animate__infinite animate__shakeY"
              >
                <circle cx="12" cy="12" r="10"></circle>
                <polyline points="8 12 12 16 16 12"></polyline>
                <line x1="12" y1="8" x2="12" y2="16"></line>
              </svg>
              </a>
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<script>
export default {
  props: {
    pageName: String,
  },
};
</script>

<style>
header {
  background: url("~/static/herobg.jpg");
}

.scrollDown {
  --animate-duration: 8.5s;
}
</style>