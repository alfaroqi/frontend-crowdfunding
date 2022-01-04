<template>
  <div class="project-page">
    <section class="dashboard-header pt-5">
      <div class="container mx-auto relative">
        <Navbar />
      </div>
    </section>
    <section class="container mx-auto pt-8">
      <div class="flex justify-between items-center">
        <div class="w-full mr-6">
          <h2 class="text-4xl text-gray-900 mb-2 font-medium">Dashboard</h2>
        </div>
      </div>
      <div class="flex justify-between items-center">
        <div class="w-3/4 mr-6">
          <h3 class="text-2xl text-gray-900 mb-4">Campaign Details</h3>
        </div>
        <div class="w-1/4 text-right">
          <nuxt-link
            to="/dashboard/projects/create"
            class="
              bg-green-button
              hover:bg-green-button
              text-white
              font-bold
              px-4
              py-1
              rounded
              inline-flex
              items-center
            "
          >
            Edit
          </nuxt-link>
        </div>
      </div>
      <div class="block mb-2">
        <div class="w-full lg:max-w-full lg:flex mb-4">
          <div
            class="
              border border-gray-400
              bg-white
              rounded
              p-8
              flex flex-col
              justify-between
              leading-normal
            "
          >
            <div>
              <div class="text-gray-900 font-bold text-xl mb-2">
                Cari Uang Buat Gunpla
              </div>
              <p class="text-sm font-bold flex items-center mb-1">
                Description
              </p>
              <p class="text-gray-700 text-base">
                Designed to fit your dedicated typing experience. No matter what
                you like, linear, clicky or a little in between, we’ve got you
                covered with three Gateron switches options (Blue, Brown, Red).
                With a lifespan of 50 million keystroke lifespan we want to make
                sure that you experience same feedback for every keystroke.
              </p>
              <p class="text-gray-700 text-base">
                With N-key rollover (NKRO on wired mode only) you can register
                as many keys as you can press at once without missing out
                characters. It allows to use all the same media keys as
                conventional macOS.
              </p>
              <p class="text-sm font-bold flex items-center mb-1 mt-4">
                What Will Funders Get
              </p>
              <ul class="list-disc ml-5">
                <li>Equity of the startup directly from the founder</li>
                <li>Special service or product that startup has</li>
                <li>
                  You can also sell your equity once the startup going IPO
                </li>
              </ul>
              <p class="text-sm font-bold flex items-center mb-1 mt-4">Price</p>
              <p class="text-4xl text-gray-700 text-base">200.000</p>
            </div>
          </div>
        </div>
      </div>
      <div class="flex justify-between items-center">
        <div class="w-3/4 mr-6">
          <h3 class="text-2xl text-gray-900 mb-4 mt-5">Gallery</h3>
        </div>
        <div class="w-1/4 text-right">
          <a
            href="#"
            class="
              bg-green-button
              hover:bg-green-button
              text-white
              font-bold
              px-4
              py-1
              rounded
              inline-flex
              items-center
            "
          >
            Upload
          </a>
        </div>
      </div>
      <div class="flex -mx-2">
        <div
          class="relative w-1/4 bg-white m-2 p-2 border border-gray-400 rounded"
        >
          <figure class="item-thumbnail">
            <img src="/project-slider-1.jpg" alt="" class="rounded w-full" />
          </figure>
        </div>
        <div
          class="relative w-1/4 bg-white m-2 p-2 border border-gray-400 rounded"
        >
          <figure class="item-thumbnail">
            <img src="/project-slider-2.jpg" alt="" class="rounded w-full" />
          </figure>
        </div>
        <div
          class="relative w-1/4 bg-white m-2 p-2 border border-gray-400 rounded"
        >
          <figure class="item-thumbnail">
            <img src="/project-slider-3.jpg" alt="" class="rounded w-full" />
          </figure>
        </div>
        <div
          class="relative w-1/4 bg-white m-2 p-2 border border-gray-400 rounded"
        >
          <figure class="item-thumbnail">
            <img src="/project-slider-4.jpg" alt="" class="rounded w-full" />
          </figure>
        </div>
      </div>
      <div class="flex justify-between items-center">
        <div class="w-3/4 mr-6">
          <h3 class="text-2xl text-gray-900 mb-4 mt-5">Transaction History</h3>
        </div>
      </div>
      <div class="block mb-2">
        <div class="w-full lg:max-w-full lg:flex mb-4" v-for="i in 5" :key="i">
          <div
            class="
              w-full
              border border-gray-400
              lg:border-gray-400
              bg-white
              rounded
              p-8
              flex flex-col
              justify-between
              leading-normal
            "
          >
            <div>
              <div class="text-gray-900 font-bold text-xl mb-1">
                Galih Pratama
              </div>
              <p class="text-sm text-gray-600 flex items-center mb-2">
                Rp. 200.000 &middot; 12 September 2020
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <div class="cta-clip -mt-20"></div>
    <section class="call-to-action bg-purple-progress pt-64 pb-10"></section>
    <Footer />
  </div>
</template>