<template>
  <main>
    <div class="container mx-auto debug">
      <section>
        <div class="text-center">
          <h1>The App for Pubs and Bars</h1>
        </div>
        <div class="text-center">
          <a href="">Get started</a>
        </div>
        <div class="text-center">
          <p>Powered by <span class="uppercase">Heineken</span></p>
        </div>
        <PillList />
      </section>

      <section>
        <div class="xl:grid xl:grid-cols-12 debug">
          <div class="x:col-start-1 xl:col-span-4">
            <PlansAndPricing />
          </div>

          <div class="xl:hidden">
            <table>
              <caption class="sr-only">
                Comparisson table
              </caption>
              <tr>
                <td></td>
                <th>Swifty Standard</th>
                <th>Swifty Plus</th>
              </tr>
              <tr>
                <td>Get started in 72hrs</td>
                <td>icon</td>
                <td>icon</td>
              </tr>
              <tr>
                <td>Order at table</td>
                <td>icon</td>
                <td>icon</td>
              </tr>
              <tr>
                <td>Loyalty campaigns</td>
                <td>icon</td>
                <td>icon</td>
              </tr>
              <tr>
                <td>Vouchers</td>
                <td>icon</td>
                <td>icon</td>
              </tr>
              <tr>
                <td>Point store</td>
                <td>icon</td>
                <td>icon</td>
              </tr>
              <tr>
                <td>Reservation management</td>
                <td>icon fade</td>
                <td>icon</td>
              </tr>
              <tr>
                <td>Mailshot feature</td>
                <td>icon fade</td>
                <td>icon</td>
              </tr>
              <tr>
                <td>Take deposits for bookings</td>
                <td>icon fade</td>
                <td>icon</td>
              </tr>
              <tr>
                <td>Limit table bookings</td>
                <td>icon fade</td>
                <td>icon</td>
              </tr>
              <tr>
                <td>Offer gift cards</td>
                <td>icon fade</td>
                <td>icon fade</td>
              </tr>
              <tr>
                <td>No onboarding fee Payments 1% +10p</td>
                <td>&pound;49 p/m</td>
                <td>&pound;169 p/m</td>
              </tr>
            </table>
          </div>

          <div class="hidden xl:block xl:col-start-6 xl:col-span-3">
            <h4>Swifty <span class="sr-only">Standard</span></h4>
            <h5>Powered by <span class="uppercase">Heineken</span></h5>
            <ul role="list">
              <li>&pound;49 p/m No onboarding fee Payments 1% +10p</li>
              <li>Get started in 72hrs</li>
              <li>Order at table</li>
              <li>Loyalty campaigns</li>
              <li>Vouchers</li>
              <li>Point store</li>
            </ul>
          </div>

          <div class="hidden xl:block xl:col-start-9 xl:col-span-3">
            <h4>Swifty <span class="sr-only">Plus</span></h4>
            <h5>Powered by <span class="uppercase">Heineken</span></h5>
            <ul role="list">
              <li>&pound;169 p/m No onboarding fee Payments 1% +10p</li>
              <li>Get started in 72hrs</li>
              <li>Order at table</li>
              <li>Loyalty campaigns</li>
              <li>Vouchers</li>
              <li>Point store</li>
              <li>Reservation management</li>
              <li>Mailshot feature</li>
              <li>Take deposits for bookings</li>
              <li>Limit table bookings</li>
            </ul>
          </div>
        </div>
      </section>
    </div>
  </main>
</template>

<script>
import PillList from "@/components/PillList";
import PillList from "@/components/PillList";

export default {
  name: "Index",
  components: {
    PillList,
  },
  metaInfo() {
    return {
      title: "Homepage • Swifty",
    };
  },
  methods: {},
};
</script>
