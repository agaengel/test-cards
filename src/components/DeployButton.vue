<template>
  <div>
    <a
      :href="
                'https://buildwith.ionos.com/setup?repo=' + url
              "
      rel="noopener"
      target="_blank"
    >
      <button
        class="text-white font-bold rounded-full bg-blue-600 inline-flex items-center shadow-lg focus:outline-none px-8 my-6 py-4"
      >
        <svg
          class="fill-current text-white w-4 h-4 mr-2"
          role="img"
          aria-hidden="true"
          xmlns="http://www.w3.org/2000/svg"
        >
          <use
            xmlns:xlink="http://www.w3.org/1999/xlink"
            xlink:href="/icons.svg#icon-ship"
          />
        </svg>
        <span>Ship {{ title }} to IONOS</span>
      </button>
    </a>
  </div>
</template>

<script>
export default {
  name: 'DeployButton',
  props: {
    url: {
      type: String,
    },
    title: {
      type: String,
    },

  },
}
</script>
