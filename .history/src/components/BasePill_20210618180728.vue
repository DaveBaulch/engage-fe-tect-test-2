<template>
  <span class="inline-block w-full md:w-21.25">
    <span
      class="
        flex flex-row
        justify-left
        bg-white bg-opacity-95
        px-5.5
        py-4.125
        rounded-basePill
        md:shadow-2xl
      "
    >
      <span class="flex flex-col justify-center mr-4 align-center">
        <BaseTickIcon />
      </span>
      <span class="text-lg font-bold text-midnight">{{ text }}</span>
    </span>
  </span>
</template>

<script>
import BaseTickIcon from "@/components/BaseTickIcon";

export default {
  name: "BasePill",
  components: {
    BaseTickIcon,
  },
  props: {
    text: {
      type: String,
      default: "",
      required: true,
    },
  },
};
</script>
