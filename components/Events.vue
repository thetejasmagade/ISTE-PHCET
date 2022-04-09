<template>
  <div class="mb-8 px-5 md:px-0">
    <h1
      class="
        text-5xl
        font-extrabold
        text-transparent
        bg-clip-text bg-gradient-to-br
        from-yellow-400
        to-red-600
        pt-8
        text-center
        pb-8
      "
      style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
    >
      Upcoming Events
    </h1>
    <div class="grid md:grid-cols-2 grid-cols-1 gap-4 container mx-auto">
      <div class="flex justify-center">
        <div
          class="
            flex flex-col
            md:flex-row md:max-w-xl
            rounded-lg
            bg-white
            shadow-lg
          "
        >
          <img
            class="
              w-full
              h-96
              md:h-auto
              object-cover
              md:w-48
              rounded-t-lg
              md:rounded-none md:rounded-l-lg
            "
            src="~/static/poster1.jpg"
            alt=""
          />
          <div class="p-6 flex flex-col justify-start">
            <h5 class="text-gray-900 text-xl font-medium mb-2">
              IOE Exhibition
            </h5>
            <p class="text-gray-700 text-base mb-4">
              IoT India expo showcases organizations leading the way in IoT adoption, enabling them to propel into a new world of business quicker, with more accurate data, ensuring their business can thrive through new technology adoptions.
            </p>
            <p class="text-gray-600 text-xs">26 March, 2022</p>
          </div>
        </div>
      </div>
      <!-- ... -->
      <div class="flex justify-center">
        <div
          class="
            flex flex-col
            md:flex-row md:max-w-xl
            rounded-lg
            bg-white
            shadow-lg
          "
        >
          <img
            class="
              w-full
              h-96
              md:h-auto
              object-cover
              md:w-48
              rounded-t-lg
              md:rounded-none md:rounded-l-lg
            "
            src="~/static/poster2.png"
            alt=""
          />
          <div class="p-6 flex flex-col justify-start">
            <h5 class="text-gray-900 text-xl font-medium mb-2">
              Ethical Hacking Workshop
            </h5>
            <p class="text-gray-700 text-base mb-4">
              Hacking is not about the illegal things it's all about how to secure your cyberspace and system from attacks.
            </p>
            <p class="text-gray-600 text-xs">29 April, 2022</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>