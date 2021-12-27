<template>
  <div class="container mx-auto h-screen flex justify-center items-center">
    <div class="w-full lg:w-1/3 px-10 lg:px-0">
      <div class="flex justify-center items-center mx-auto mt-6 mb-8">
        <img src="/success-illustration.svg" alt="" class="w-full" />
      </div>
      <h2 class="font-medium mb-3 text-3xl text-center">Welcome onboard!</h2>
      <p class="text-center font-light">
        Your account just registered
        <br />
        into our system
      </p>
      <div class="mb-4 mt-6">
        <div class="mb-3">
          <button
            @click="$router.push({ path: '/' })"
            class="
              block
              w-full
              bg-orange-button
              hover:bg-green-button
              text-white
              font-semibold
              px-6
              py-4
              text-lg
              rounded-full
            "
          >
            Start Explore
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: 'success',
}
</script>


