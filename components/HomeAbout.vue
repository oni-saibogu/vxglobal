<script lang="ts" setup>
const [visible, container] = useVisible();
</script>
<template>
  <div
    ref="container"
    class="relative flex flex-col md:relative md:h-md md:justify-end md:pt-16 lg:-translate-y-16 2xl:h-2xl 4xl:h-4xl 2xl:w-9/10 2xl:pb-24"
  >
    <div
      :class="visible ? 'animate-slide-in-left visible' : 'invisible'"
      class="relative flex flex-col 2xl:w-9/10 2xl:self-center"
    >
      <div
        class="absolute inset-0 bg-black max-w-7/10 blur-2xl lt-md:max-w-xs md:blur-3xl"
      />
      <div
        class="flex flex-col space-y-4 z-10 px-2 lt-md:pb-8 md:px-8 lg:px-16 md:space-y-4 2xl:px-0"
      >
        <div
          class="leading-relaxed lt-md:max-w-xs md:max-w-auto md:leading-loose"
        >
          <p>
            Founded in 2011, VX GLOBAL began as a distribution company in
            <br class="lt-md:hidden" />
            the FMCG (Fast Moving Consumer Goods) segment in Singapore.<br
              class="lt-md:hidden"
            />
            The company has since grown with its primary business pivoting
            <br class="lt-md:hidden" />
            to Fund services and portfolio management, <br class="md:hidden" />
            it is also involved in
            <br class="lt-md:hidden" />
            the acceleration of startups across Southeast Asia.
          </p>
        </div>
        <div class="self-start flex flex-col">
          <NuxtLink to="/about-us">
            <ButtonOutlineFill class="bg-primary/50 md:px-8 md:py-4">
              <p class="text-white/70 p-4">Read more</p>
            </ButtonOutlineFill>
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>
