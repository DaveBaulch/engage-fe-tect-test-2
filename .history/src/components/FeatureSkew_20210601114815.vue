<template>
  <div
    class="
      pt-skew
      rounded-featureSkew
      bg-gradient-to-r
      from-lightLavender-light
      to-lightLavender-dark
      skew
      debug
      scale-55
      xl-scale-100
    "
  ></div>
</template>

<script>
export default {
  name: "FeatureSkew",
};
</script>

<style>
.skew {
  transform: perspective(100em) translateX(-108px) rotateY(-29deg);
  width: 116%;
}
</style>
