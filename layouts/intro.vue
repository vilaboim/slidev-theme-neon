<template>
  <section class="slidev-layout intro">
    <article class="my-auto w-full">
      <slot />
      <div class="flex justify-between items-end gap-2">
        <div>
          <slot name="content" />
        </div>

        <figure class="relative overflow-hidden w-1/3 p-[5px] rounded">
          <span class="absolute -inset-[50%] w-[200%] bg-gradient-to-r from-[#6B53D9] dark:from-[#FFF] to-[#624284] dark:to-[#CCC] animate-spin" />
          <img
            class="relative"
            :src="$attrs.photo"
          />
        </figure>
      </div>
    </article>
  </section>
</template>
