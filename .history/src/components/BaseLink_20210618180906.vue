<template>
  <router-link v-if="type === 'router-link'" :to="to" class="inline-block">
    <span
      class="
        bg-midnight
        rounded-baseLink
        flex flex-row
        justify-center
        px-10
        py-6
      "
    >
      <span class="text-lg font-bold text-white">{{ text }}</span>
      <span class="align-center flex flex-col justify-center ml-2">
        <SpriteIcon
          name="chevronRight"
          class="text-lightLavender-light w-1.5 h-3"
        />
      </span>
    </span>
  </router-link>
  <a v-else-if="type === 'link'" :href="to" class="inline-block">
    <span
      class="
        bg-midnight
        rounded-baseLink
        flex flex-row
        justify-center
        px-10
        py-6
      "
    >
      <span class="text-lg font-bold text-white">{{ text }}</span>
      <span class="align-center flex flex-col justify-center ml-2">
        <SpriteIcon
          name="chevronRight"
          class="text-lightLavender-light w-1.5 h-3"
        />
      </span>
    </span>
  </a>
</template>

<script>
import SpriteIcon from "@/components/SpriteIcon";

export default {
  name: "BaseLink",
  components: {
    SpriteIcon,
  },
  props: {
    type: {
      type: String,
      default: "router-link",
      required: false,
    },
    to: {
      type: String,
      default: "",
      required: true,
    },
    text: {
      type: String,
      default: "",
      required: true,
    },
  },
};
</script>
