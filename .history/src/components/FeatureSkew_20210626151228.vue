<template>
  <div class="gsap-skew relative z-0">
    <div
      class="
        pt-skew
        rounded-featureSkew
        bg-gradient-to-r
        from-lightLavender-light
        to-lightLavender-dark
        skew
        debug
        md:ml-0
        relative
        z-10
        ml-16
      "
    ></div>
    <div
      class="
        pt-skew
        rounded-featureSkew
        bg-appBlue
        opacity-10
        skew
        debug
        md:ml-0
        left-4
        top-4
        md:left-7
        md:top-7
        absolute
        ml-16
      "
    ></div>
  </div>
</template>

<script>
import prefersReducedMotion from "@/mixins/prefersReducedMotion";
import gsap from "gsap";

export default {
  name: "FeatureSkew",
  mixins: [prefersReducedMotion],
  methods: {
    animateSkew() {
      const animationIsOkay = this.prefersReducedMotion();
      if (animationIsOkay) {
        gsap.fromTo(
          ".gsap-skew",
          {
            opacity: 0,
          },
          {
            opacity: 1,
            duration: 4,
          }
        );
      }
    },
  },

  mounted() {
    this.animateSkew();
  },
};
</script>
