<template>
  <div>
    <div class="animate move">
      <img :src="require('@/assets/animation.gif')" alt="Kusama" />
      <p class="marquee"><span>Subscribe</span></p>
      <div>
        <button
          class="btn bg-transparent text-red-600 text-sm px-2 py-1 border border-red-400 rounded"
        >
          Subscribe for Updates
        </button>
      </div>
    </div>

    <p class="max-w-md  md:text-4xl text-xl font-bold mr-auto mt-24 mb-5">
      The Scalable, Multichain Network for Radical Innovation.
    </p>
    <p class="max-w-2xl text-md text-white font-semibold leading-loose ml-auto">
      Unprecedented interoperability and scalability for blockchain developers
      who want to quickly push the limits of what’s possible. Buil''t using
      Substrate with nearly the same codebase and industry-leading multichain
      infrastructure as Kusama’s cousin, Polkadot.
    </p>
    <div class="mt-24 flex justify-center">
      <img src="@/assets/boxes_graph.png" alt="" />
    </div>

    <div class="mt-12">
      <p class="mr-auto text-xl md:text-4xl font-bold mb-5">
        Origin of Kusama
      </p>
      <p class="mr-auto max-w-md text-md font-semibold leading-loose">
        The relationship between society and technology has deteriorated to the
        point where large entities routinely stretch and overstep their
        authority.
      </p>
      <p class="text-md max-w-md font-semibold  leading-loose mt-5">
        Kusama is a network built as a risk-taking, fast-moving ‘canary in the
        coal mine’ for its cousin Polkadot. It's a living platform built for
        change agents to take back control, spark innovation and disrupt the
        status quo.
      </p>
    </div>

    <div class="mt-12 paralax max-w-2xl ml-auto">
      <div class="box-outlines" style="--progress:44%">
        <div>
          <p class=" text-lg md:text-4xl text-white font-bold">
            What is Kusama?
          </p>
          <p class=" mt-4 text-md text-white font-semibold leading-loose">
            Kusama is a scalable network of specialized blockchains built using
            Substrate and nearly the same codebase as Polkadot. The network is
            an experimental development environment for teams who want to move
            fast and innovate on Kusama, or prepare for deployment on Polkadot.
          </p>
          <p class=" mt-3 text-md text-white font-semibold leading-loose">
            Kusama was founded in 2019 by Gavin Wood, founder of Polkadot and
            co-founder and former CTO of Ethereum.
          </p>
        </div>
      </div>
    </div>
    <div class="mt-24">
      <div class="grid-7">
        <div class="item1 mr-auto text-xl md:text-4xl font-bold">
          Launch your custom blockchain
        </div>
        <div class="item2">
          <img src="@/assets/mesh_graph_1.png" />
        </div>
        <div class="item3 scroll_hide_bar">
          <ul>
            <div v-for="item in dados1" :key="item.id">
              <li class="text-xl md:text-4xl font-bold mb-6">
                {{ item.text }}
              </li>
              <div class="mb-6">{{ item.subtext }}</div>
            </div>
          </ul>
        </div>
      </div>
    </div>
    <div class="mt-12 text-center">
      <button
        class="bg-transparent   text-red-600 text-sm px-2 py-1 border border-red-400 rounded
           hover:text-blue-600 hover:border-blue-400"
      >
        Ready to Start? Contact Our Team.
      </button>
    </div>

    <section class="grid-8 mt-12">
      <div class="item1  text-xl md:text-4xl font-bold mb-3">
        Bring Inovation to your Project
      </div>
      <div class="item2 scroll_hide_bar">
        <div class="text-md text-white font-semibold leading-loose">
          <ul>
            <li class="text-md md:text-4xl text-white font-bold mb-3">
              Innovation
            </li>
            <p>
              Innovation Kusama is built by the same teams as Polkadot, using
              nearly the same code and tools. The network places the latest tech
              from Parity Technologies and Web3 Foundation in the hands of
              developers, even before those features make it to Polkadot.
            </p>

            <li class="text-md md:text-4xl text-white font-bold  mb-3 mt-6">
              Scalability
            </li>
            <p>
              Kusama’s sharded blockchains and open governance provide a
              scalable and future-proof infrastructure for businesses,
              marketplaces and applications to deploy and mature.
            </p>

            <li class="text-md md:text-4xl text-white font-bold  mb-3  mt-6">
              Interoperability
            </li>
            <p>
              Kusama brings multiple blockchains together into one sharded
              network, freeing developers from the siloes created by legacy
              blockchain networks.
            </p>

            <li class="text-md md:text-4xl text-white font-bold  mb-3 mt-6 ">
              Customization
            </li>
            <p>
              With Substrate, developers can build their own app-specific
              blockchain and connect it to Kusama.
            </p>
          </ul>
        </div>
      </div>
    </section>

    <section class="grid-9 mt-12">
      <div class="item1 text-xl md:text-4xl text-white font-bold">
        Develop on the Canary Network
      </div>
      <div class="item2">
        <img src="@/assets/mesh_graph_2.png" />
      </div>
      <p class="item3 md:text-xl text-white font-bold">
        Many teams will choose Kusama for their dapp or parachain and remain
        exclusively on Kusama. Other teams will join Kusama as a temporary
        preparation ground for deployment on Polkadot.
      </p>
    </section>
    <div
      class="item1 text-center mt-12 text-xl md:text-4xl text-white font-bold"
    >
      Join the Kusama Ecosystem
    </div>

    <div class="grid-10 mt-6">
      <div v-for="item in cards" :key="item.id">
        <Icon :icon="item.icon" :title="item.title" />
      </div>
    </div>

    <div class="grid-11 mt-12">
      <div class="item1  text-xl md:text-3xl text-white font-bold">
        Parachains and Applications
      </div>
      <div class="item2 scroll_hide_bar">
        <div class=" mt-3">
          <ul>
            <li
              v-for="soc in social"
              :key="soc.id"
              class="text-md md:text-xl text-white font-bold mb-3"
            >
              {{ soc.title }}
            </li>
          </ul>
        </div>
      </div>
    </div>
    <div class="text-center mt-12">
      <button
        class="bg-transparent  text-red-600 text-sm px-2 py-1 border border-red-400 rounded
           hover:text-blue-600 hover:border-blue-400"
      >
        Why Build a Parachain
      </button>
    </div>
    <div class="mt-12">
      <div class="grid-11">
        <div class="item1  text-md md:text-3xl text-white font-bold">
          KSM Token Utilization
        </div>
        <div class="item2 scroll_hide_bar">
          <div class="mt-3">
            <ul>
              <li
                v-for="item in dados4"
                :key="item.id"
                class="text-md md:text-xl text-white font-bold mb-3"
              >
                {{ item.caps }}
                <span class="text-sm md:text-md  font-semibold text-gray-500">{{
                  item.text
                }}</span>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>

    <div class="grid-11 mt-12">
      <div class="item1 text-xl md:text-3xl text-white font-bold">
        Built with Substrate
      </div>
      <div class="item2 scroll_hide_bar">
        <img
          src="@/assets/substrate-playground.png"
          alt="Substrate Playground"
          width="100%"
          class="mb-4"
        />
        <div>
          Your Substrate Blockchain is natively compatible with Kusama, making
          it simple to secure your blockchain and communicate with Kusama's
          network.`
        </div>
        <div class="flex text-center mt-6 justify-left">
          <button
            class="bg-transparent  text-red-600 text-sm px-2 py-1 border border-red-400 rounded
           hover:text-blue-600 hover:border-blue-400"
          >
            Learn More
          </button>
          <button
            class="bg-transparent  text-red-600 text-sm px-2 py-1 border border-red-400 rounded
           hover:text-blue-600 hover:border-blue-400 ml-6"
          >
            Substract Playground
          </button>
        </div>
      </div>
    </div>
    <div class="text-center text-xl md:text-3xl text-white font-bold mt-24">
      Take Flight
    </div>

    <div class="mt-12 paralax grid-12">
      <div
        v-for="item in dados5"
        :key="item.id"
        class="box-outlines"
        style="--progress:44%"
      >
        <p class="text-md md:text-xl font-bold mb-3">{{ item.title }}</p>
        <ul>
          <li
            v-for="dta in item.listData"
            :key="dta.title"
            class="flex justify-between"
          >
            <div>{{ dta.title }}</div>
            <div><i class="material-icons text-2xl">arrow_forward </i></div>
          </li>
        </ul>
      </div>
    </div>
    <div
      class="text-center max-w-md text-xl md:text-3xl text-white font-bold mt-12 mx-auto"
    >
      Stay in the Loop
    </div>
    <div
      class="text-center max-w-sm text-sm md:text-md  text-white font-bold mt-3 mx-auto"
    >
      Subscribe to the newsletter to hear about Kusama updates and events.
    </div>
    <div class="text-center mt-6">
      <button
        class="bg-transparent  text-red-600 text-sm font-bold px-2 py-1 border border-red-400 rounded
           hover:text-blue-600 hover:border-blue-400"
      >
        Subscribe
      </button>
    </div>

    <div class="text-center mt-6">
      <p class="text-center max-w-sm text-xs text-white font-bold mt-6 mx-auto">
        To see how we use your information please see our privacy policy.
      </p>
    </div>
    <div class="mt-24">
      <div class="grid-13">
        <div v-for="item in dados6" :key="item.id">
          <div class="text-xl md:text-2xl text-white font-bold mb-2">
            {{ item.title }}
          </div>
          <div
            v-for="dta in item.listData"
            :key="dta.title"
            class="text-sm md:text-md mb-1"
          >
            {{ dta.title }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Icon from "./Icon";
export default {
  name: "Content",
  components: { Icon },
  data: () => ({
    social: [
      {
        id: 1,
        title: "Gaming and eSports",
      },
      {
        id: 2,
        title: "Messaging",
      },
      {
        id: 3,
        title: "DAO",
      },
      {
        id: 4,
        title: "Marketplaces",
      },
      {
        id: 5,
        title: "Oracles",
      },
      {
        id: 6,
        title: "Music",
      },
      { id: 7, title: "Social Networking" },
    ],
    cards: [
      {
        icon: "airplay",
        title: "Polkadot",
      },
      {
        icon: "alarm",
        title: "Acala",
      },
      {
        icon: "card_travel",
        title: "Chainlink",
      },

      {
        icon: "manage_accounts",
        title: "Moonbeam",
      },

      {
        icon: "next_plan",
        title: "Phala",
      },

      {
        icon: "outbox",
        title: "Edgeware",
      },
    ],
    dados4: [
      {
        id: 1,
        caps: "Validate ",
        text: "the network",
      },
      {
        id: 2,
        caps: "Nominate ",
        text: "validators",
      },
      {
        id: 3,
        caps: "Bond ",
        text: "parachains or parathreads",
      },

      {
        id: 4,
        caps: "Vote ",
        text: "on governance referenda",
      },
    ],
    dados1: [
      {
        id: 1,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Fast Iteration",
        subtext:
          "Move fast and ship your product. Kusama’s risk-taking and nimble mentality allows developers to move swiftly through the governance and upgrade process, enabling rapid progress and growth.",
      },

      {
        id: 2,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Low Economic Barriers",
        subtext:
          "Launch your custom blockchain (parachain) project with low barriers to entry. Ideal for lean startups looking to move fast and iterate.",
      },

      {
        id: 3,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Advanced Technology",
        subtext:
          "Build on a next-generation, sharded, multichain network, while employing the newest features before they are deployed on Polkadot.",
      },

      {
        id: 4,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Open Governance",
        subtext:
          "Kusama is owned and governed by a community of network participants who vote on and control the evolution of the network. Have a voice and make your mark in the evolution of the network.",
      },

      {
        id: 5,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Engaged Community",
        subtext:
          "Leverage Polkadot’s global brand and developer community for your parachain, parathread or dApp.",
      },
      {
        id: 6,
        icon:
          "data:image/svg+xml,%3Csvg%20width%3D%2240%22%20height%3D%2240%22%20viewBox%3D%220%200%2040%2040%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%3Ctitle%3Efast%3C%2Ftitle%3E%3Cpath%20d%3D%22M0%2020v-.59c0-.328.266-.586.594-.586h1.165c.333%200%20.594.265.594.593V20c0%209.746%207.9%2017.647%2017.647%2017.647h.593c.316%200%20.583.266.583.594v1.165c0%20.333-.265.594-.593.594H20C8.954%2040%200%2031.046%200%2020zm40%200v.586c0%20.323-.266.59-.594.59h-1.165c-.333%200-.594-.265-.594-.593V20c0-9.746-7.9-17.647-17.647-17.647h-.586c-.33%200-.59-.266-.59-.594V.594c0-.333.263-.594.588-.594H20c11.046%200%2020%208.954%2020%2020zm-20%208.235c-4.548%200-8.235-3.687-8.235-8.235s3.687-8.235%208.235-8.235%208.235%203.687%208.235%208.235-3.687%208.235-8.235%208.235z%22%20fill%3D%22%23FFF%22%20fill-rule%3D%22nonzero%22%2F%3E%3C%2Fsvg%3E",
        text: "Valuable Experience",
        subtext:
          "For teams looking to move to Polkadot after fine-tuning on Kusama, begin building your community and brand on Kusama before deployment.",
      },
    ],
    dados5: [
      {
        id: 1,
        title: "Build",
        listData: [
          { id: 1, title: "Kusama Docs", icon: "mdi-arrow-right" },
          { id: 2, title: "Learn Substrate", icon: "mdi-arrow-right" },
        ],
      },
      {
        id: 2,
        title: "Validate",
        icon: "",
        listData: [
          { id: 1, title: "Start Validating", icon: "mdi-arrow-right" },
          { id: 2, title: "Technical Updates", icon: "mdi-arrow-right" },
        ],
      },
      {
        id: 3,
        title: "Join",
        icon: "",
        listData: [
          { id: 1, title: "Ambassador Program", icon: "mdi-arrow-right" },
          { id: 2, title: "Nominate a Validator", icon: "mdi-arrow-right" },
        ],
      },
    ],
    dados6: [
      {
        id: 1,
        title: "Developers",
        listData: [
          { id: 1, title: "Guide" },
          { id: 2, title: "GitHub" },
          { id: 3, title: "Technical Riot Chat" },
          { id: 4, title: "Web3 Foundation Grants" },
          { id: 5, title: "Governance Chat" },
          { id: 6, title: "Validator Chat" },
        ],
      },
      {
        id: 2,
        title: "Community",
        listData: [
          { id: 1, title: "Community Hub" },
          { id: 2, title: "Ambassador Program" },
          { id: 3, title: "Meetup Hub" },
          { id: 4, title: "Find a Local Meetup" },
          { id: 5, title: "Blog" },
          { id: 6, title: "Brand Assets" },
        ],
      },
      {
        id: 3,
        title: "Social",
        listData: [
          { id: 1, title: "Discord" },
          { id: 2, title: "Watercooler Riot Chat" },
          { id: 3, title: "Twitter" },
          { id: 4, title: "Reddit" },
          { id: 5, title: "YouTube" },
          { id: 6, title: "Crowdcast Webinars" },
        ],
      },
      {
        id: 4,
        title: "Info",
        listData: [
          { id: 1, title: "Support" },
          { id: 2, title: "Polkadot" },
          { id: 3, title: "Substrate" },
          { id: 4, title: "Careers" },
          { id: 5, title: "Web3 Foundation" },
          { id: 6, title: "Parity Technologies" },
        ],
      },
    ],
  }),
};
</script>

<style lang="scss">
/* animate img div butto*/
.animate {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: repeat(1, 1fr);
  row-gap: 20px;
  max-width: 70%;
  margin: 0 auto;
  justify-items: center;

  img {
    grid-column: 1;
    grid-row: 1 / 3;
  }

  .marquee {
    grid-column: 1;
    grid-row: 1;
    /* background: green; */
    align-self: end;
  }
  button {
    grid-column: 1;
    grid-row: 2;
    /* background: green; */
    align-self: end;
    justify-self: center;
  }
}

.marquee {
  margin: 0 auto;
  white-space: nowrap;
  overflow: hidden;
  max-width: 300px;
}
.marquee span {
  display: inline-block;
  color: white;
  padding-left: 40%;
  animation: marquee 5s linear infinite;
}
@keyframes marquee {
  to {
    transform: translateX(-100%);
  }
}

/* box-outlines */
.box-outlines {
  display: inline-block;
  width: auto;
  position: relative;
  padding: 2rem 3rem !important;
}
.box-outlines::before,
.box-outlines::after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  border: solid 2px red;
  pointer-events: none;
}
.parallax .box-outlines::after {
  transform: translate3d(
    calc(var(--progress) / 20),
    calc(var(--progress) / 20),
    0
  );
}
.box-outlines::before {
  transform: translate3d(
    calc(var(--progress) / 20 * -1),
    calc(var(--progress) / 20 * -1),
    0
  );
}

/* grid-7 */
.grid-7 {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(80px, 1fr));
  justify-content: center;
  margin: 0 auto;
}
.grid-7 .item1 {
  grid-row: 1 / 1;
  grid-column: 2 / 6;
  z-index: 1;
  margin-top: 40px;
}
.grid-7 .item2 {
  grid-row: 1 / 1;
  grid-column: 3 / -1;
}
.grid-7 .item2 img {
  grid-row: 1 / -1;
  max-width: 100%;
}
.grid-7 .item3 {
  grid-row: 1 / -1;
  grid-column: 7 / -1;
}

@media only screen and (max-width: 768px) {
  .grid-7 .item1 {
    grid-row: 1 / 1;
    grid-column: 2 / 4;
    z-index: 1;
    margin-top: 40px;
  }
  .grid-7 .item3 {
    grid-row: 1 / 1;
    grid-column: 5 / -1;
  }
}

@media only screen and (max-width: 600px) {
  .grid-7 {
    display: block;
  }
}

.grid-8 {
  display: grid;
  grid-template-columns: minmax(300px, 1fr) auto;
  column-gap: 150px;
}
.grid-8 .item1 {
  grid-row: 1;
  grid-column: 1;
  max-width: 500px;
}
.grid-8 .item2 {
  grid-row: 1;
  grid-column: 2;
  height: 50vh;
  overflow-y: scroll;
}
@media only screen and (max-width: 600px) {
  .grid-8 {
    display: block;
  }
}
.grid-9 {
  display: grid;
  grid-template-columns: repeat(6, minmax(80px, 1fr));
}
.grid-9 .item1 {
  grid-row: 1 / 1;
  grid-column: 1 / 3;
  z-index: 1;
  margin-top: 40px;
}
.grid-9 .item2 {
  grid-row: 1 / 1;
  grid-column: 2 / -1;
}
.grid-9 .item2 img {
  grid-row: 1 / -1;
  grid-column: 2 / -1;
}
.grid-9 .item3 {
  grid-row: 1 /-1;
  grid-column: 3 / -1;
  align-self: end;
  justify-self: start;
  margin-bottom: 30px;
}

@media only screen and (max-width: 600px) {
  .grid-9 {
    display: block;
  }
}
.grid-10 {
  display: grid;
  grid-template-columns: repeat(6, minmax(80px, 1fr));
  justify-content: center;
  align-items: center;
}

@media only screen and (max-width: 600px) {
  .grid-10 {
    grid-template-columns: repeat(3, minmax(80px, 1fr));
    row-gap: 10px;
  }
}

.grid-11 {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
}
.grid-11 .item1 {
  grid-row: 1;
  grid-column: 1;
}

.grid-11 .item2 {
  grid-row: 1;
  grid-column: 2/-1;
}
@media only screen and (max-width: 600px) {
  .grid-11 {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    column-gap: 10px;
  }
}

.grid-12 {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  column-gap: 20px;
}

@media only screen and (max-width: 768px) {
  .grid-12 {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    row-gap: 10px;
  }
}

@media only screen and (max-width: 600px) {
  .grid-12 {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    row-gap: 10px;
  }
}

.grid-13 {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(80px, 1fr));
  column-gap: 30px;
  justify-content: left;
  margin: 0 auto;
}

@media only screen and (max-width: 600px) {
  .grid-13 {
    grid-template-columns: repeat(2, minmax(80px, 1fr));
    column-gap: 20px;
    row-gap: 20px;
  }
}

/* Chrome, Safari and Opera */
/* .no-scrollbar::-webkit-scrollbar {
  display: none;
}
*/

// .no-scrollbar {
//   -ms-overflow-style: none;  // IE and Edge
//   scrollbar-width: none; // Firefox
// }

.scroll_hide_bar {
  /* width: 200px; */
  max-height: 500px;
  /* border: 1px dotted black; */
  overflow-y: scroll; /* Add the ability to scroll */
}

/* Hide scrollbar for Chrome, Safari and Opera */
.scroll_hide_bar::-webkit-scrollbar {
  display: none;
}

/* Hide scrollbar for IE, Edge and Firefox */
.scroll_hide_bar {
  -ms-overflow-style: none; /* IE and Edge */
  scrollbar-width: none; /* Firefox */
}

/* .move {
  transition: 0.2s;
}
.move:hover {
  opacity: 0;
  transform: scale(5) rotate(30deg);
  -moz-transform: scale(5) rotate(30deg);
  -webkit-transform: scale(5) rotate(30deg);
  -o-transform: scale(5) rotate(30deg);
} */
</style>
