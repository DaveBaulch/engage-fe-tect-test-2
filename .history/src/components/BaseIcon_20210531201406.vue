<template>
  <div
    class="relative rounded-full bg-appBlue relative w-20 h-20"
  >
    <SpriteIcon
      name="check"
      class="text-white w-5 h-5 absolute top-0 right-0"
    />
  </div>
</template>

<script>
import SpriteIcon from "@/components/SpriteIcon";

export default {
  name: "BaseIcon",
  components: {
    SpriteIcon,
  },
};
</script>
