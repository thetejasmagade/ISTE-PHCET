<template>
  <div>
      <img
          src="https://cdn-icons-png.flaticon.com/512/3939/3939627.png"
          v-if="!bulbOn"
          height="200px"
          width="200px"
          class="md:mx-auto ml-36"
        />
        <img
          src="https://cdn-icons-png.flaticon.com/512/3939/3939470.png"
          v-else
          height="200px"
          width="200px"
          class="md:mx-auto ml-36"
        />

        <button
          type="button"
          @click="turnOn()"
          class="
            invisible
            md:visible
            mx-24
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
            invisible
            md:visible
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
}
</script>

<style>

</style>