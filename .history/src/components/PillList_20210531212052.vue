<template>
  <div class="transform -translate-y-pills">
    <ul role="list" class="xl:grid xl:grid-cols-2 gap-8 debug">
      <li class="place-self-end mr-32">
        <BasePill text="Order &amp; pay at table" class="pill" />
      </li>
      <li class="place-self-start ml-32">
        <BasePill text="Increase your revenue" class="pill" />
      </li>
      <li class="place-self-end mr-44">
        <BasePill text="Build customer loyalty" class="pill" />
      </li>
      <li class="place-self-start ml-44">
        <BasePill text="Reservation management" class="pill" />
      </li>
      <li class="place-self-end mr-32">
        <BasePill text="All-in-one solution" class="pill" />
      </li>
      <li class="place-self-start ml-32">
        <BasePill text="Quick setup" class="pill" />
      </li>
    </ul>
  </div>
</template>

<script>
import BasePill from "@/components/BasePill";
import prefersReducedMotion from "@/mixins/prefersReducedMotion";
import gsap from "gsap";

export default {
  name: "PillList",
  components: {
    BasePill,
  },
  mixins: [prefersReducedMotion],
  methods: {
    animatePills() {
      const animationIsOkay = this.prefersReducedMotion();
      if (animationIsOkay) {
        gsap.fromTo(
          ".pill",
          {
            y: 0,
            opacity: 0,
          },
          {
            y: -40,
            opacity: 1,
            duration: 2,
            stagger: {
              each: 1,
            },
          }
        );
      }
    },
  },
  mounted() {
    this.animatePills();
  },
};
</script>
