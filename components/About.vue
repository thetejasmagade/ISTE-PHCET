<template>
  <div id="About">
    <div id="content-mobile" class="mx-8 text-center">
      <div class="pl-16">
        <img
          src="~/static/images/bulbon.png"
          v-if="!bulbOn"
          height="200px"
          width="200px"
          class="pt-12"
        />
        <img
          src="~/static/images/bulboff.png"
          v-else
          height="200px"
          width="200px"
          class="pt-12"
        />
      </div>
      <button
        type="button"
        @click="turnOn()"
        class="
          mt-8
          text-white
          bg-yellow-400
          hover:bg-yellow-500
          focus:outline-none focus:ring-4 focus:ring-yellow-300
          font-medium
          rounded-full
          text-sm
          px-5
          py-2.5
          text-center
          mr-2
          mb-2
        "
      >
        Turn Bulb ON
      </button>
      <button
        type="button"
        @click="turnOff()"
        class="
          text-white
          bg-purple-700
          hover:bg-purple-800
          focus:outline-none focus:ring-4 focus:ring-purple-300
          font-medium
          rounded-full
          text-sm
          px-5
          py-2.5
          text-center
          mb-2
        "
      >
        Turn Bulb OFF
      </button>
    </div>
    <div class="grid grid-cols-3 gap-4">
      <div class="pt-1 md:pt-28">
        <Bulb id="content-desktop" />
      </div>
      <div class="col-span-3 md:col-span-2 container mx-auto md:px-32 px-8">
        <h1
          class="
            text-5xl
            font-extrabold
            text-transparent
            bg-clip-text bg-gradient-to-br
            from-yellow-400
            to-red-600
            pt-8
          "
          style='Inter, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue", sans-serif;'
        >
          About
        </h1>
        <p class="pt-5">
          The <b>Indian Society for Technical Education (ISTE)</b> is the
          leading National Professional non-profit making Society for the
          Technical Education System in our country with the motto of Career
          Development of Teachers and Personality Development of Students and
          overall development of our Technical Education System. Being the only
          national organisation of educators in the field of Engineering and
          Technology, ISTE effectively contributes in various missions of the
          Union Government.
          <br />
          <span id="content-desktop">
            The strength of ISTE is the strong base it has in technical
            education institutions in the country. ISTE has an Executive Council
            at National level. It has active membership of more than 128500
            technical teachers, 535000 student members, more than 2740
            institutional members (including IITs, IISc., NITs and other leading
            technical institutions), 1414 faculty chapters and 1505 students’
            chapters at National level and 19 Sections at State Level.
          </span>
        </p>
        <NuxtLink to="/about">
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
              py-1
              mt-5
              text-center
              mr-2
              mb-2
            "
          >
            Read More ...
          </button>
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      bulbOn: false,
    };
  },
  methods: {
    turnOn() {
      this.bulbOn = true;
    },
    turnOff() {
      this.bulbOn = false;
    },
  },
};
</script>

<style>
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