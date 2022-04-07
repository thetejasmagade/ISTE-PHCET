<template>
  <div class="pt-28">
    <div class="px-4 md:px-28 md:py-14 py-6 mb-0 pb-0 text-center md:text-left">
      <div class="grid grid-cols-2 md:grid-cols-3 gap-4">
        <div class="col-span-2">
          <h1
            class="font-bold text-5xl leading-tight"
            style="font-family: 'Poppins', sans-serif"
          >
            <span class="text-red-500">I</span>ndian
            <span class="text-red-500">S</span>ociety For <br /><span
              class="text-red-500"
              >T</span
            >echnical <span class="text-red-500">E</span>ducation
          </h1>
          <p class="text-xl pt-8 text-gray-700 pb-12">
            Tools tutorials, design and innovation experts, allin one place! The
            most intuitive way to imagineyour next user experience.
          </p>
          <button
            type="button"
            class="
              text-white
              bg-red-500
              hover:bg-red-400
              focus:outline-none focus:ring-4 focus:ring-red-300
              font-medium
              rounded-full
              text-base
              px-5
              py-2.5
              text-center
              mr-2
              mb-2
            "
          >
            Become a Member
          </button>
          <button
            class="
              text-white
              bg-gray-400
              hover:bg-gray-500
              focus:outline-none focus:ring-4 focus:ring-gray-300
              font-medium
              rounded-full
              text-base
              px-12
              py-2.5
              text-center
              mr-2
              mb-2
            "
          >
            Learn More
          </button>
        </div>
        <div class="flex items-center">
          <img id="content-desktop" src="~/static/images/hero-img.png" alt="" />
        </div>
      </div>
      <img
        id="content-mobile"
        class="pt-5"
        src="~/static/images/hero-img.png"
        alt=""
      />
    </div>

  </div>
</template>

<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap");

#content-desktop {
  display: block;
}
#content-mobile {
  display: none;
}
@media screen and (max-width: 768px) {
  #content-desktop {
    display: none;
  }
  #content-mobile {
    display: block;
  }
}
</style>