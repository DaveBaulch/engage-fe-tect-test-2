<template>
  <div>
    <table>
      <caption class="sr-only">
        Comparisson table
      </caption>
      <tr>
        <td></td>
        <th>
          <SpriteIcon
            name="logo"
            ariaLabel="Swifty"
            ariaHidden="false"
            class="inline-block w-12 h-1.375 text-appBlue leading-none"
          />
          <span>Standard</span>
        </th>
        <th>
          <SpriteIcon
            name="logo"
            ariaLabel="Swifty"
            ariaHidden="false"
            class="inline-block w-12 h-1.375 text-appBlue leading-none"
          />
          <span>Plus</span>
        </th>
      </tr>
      <tr>
        <td class="py-4">Get started in 72hrs</td>
        <td class="text-center"><BaseIcon /></td>
        <td><BaseIcon /></td>
      </tr>
      <tr>
        <td class="py-4">rder at table</td>
        <td><BaseIcon /></td>
        <td><BaseIcon /></td>
      </tr>
      <tr>
        <td class="py-4">Loyalty campaigns</td>
        <td><BaseIcon /></td>
        <td><BaseIcon /></td>
      </tr>
      <tr>
        <td class="py-4">Vouchers</td>
        <td><BaseIcon /></td>
        <td><BaseIcon /></td>
      </tr>
      <tr>
        <td class="py-4">Point store</td>
        <td><BaseIcon /></td>
        <td><BaseIcon /></td>
      </tr>
      <tr>
        <td class="py-4">Reservation management</td>
        <td><BaseIcon /></td>
        <td><BaseIcon /></td>
      </tr>
      <tr>
        <td class="py-4">Mailshot feature</td>
        <td><BaseIcon /></td>
        <td><BaseIcon /></td>
      </tr>
      <tr>
        <td class="py-4">Take deposits for bookings</td>
        <td><BaseIcon /></td>
        <td><BaseIcon /></td>
      </tr>
      <tr>
        <td class="py-4">Limit table bookings</td>
        <td><BaseIcon /></td>
        <td><BaseIcon /></td>
      </tr>
      <tr>
        <td class="py-4">Offer gift cards</td>
        <td><BaseIcon /></td>
        <td><BaseIcon /></td>
      </tr>
      <tr>
        <td class="py-4">No onboarding fee Payments 1% +10p</td>
        <td>&pound;49 p/m</td>
        <td>&pound;169 p/m</td>
      </tr>
    </table>
  </div>
</template>

<script>
import SpriteIcon from "@/components/SpriteIcon";
import BaseIcon from "@/components/BaseIcon";
export default {
  name: "ComparissonTable",
  components: {
    SpriteIcon,
    BaseIcon,
  },
};
</script>
