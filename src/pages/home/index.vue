<template>
  <div class="wrap-1 white-0">
    <div class="ta-c con-3">
      <div class="mt-6">
        <a href="https://dev.apebank.io" target="_blank">
          <img src="img/logo512.png" width="160" />
        </a>
      </div>

      <div class="mt-8">
        <v-btn
          large
          style="min-width: 180px"
          color="rgba(255, 255, 255, 0.25)"
          href="https://dev.apebank.io"
          target="_blank"
        >
          <b class="white-0 fz-18">Enter APP</b>
        </v-btn>
        <v-btn
          large
          class="ml-5"
          color="rgba(255, 255, 255, 0.25)"
          href="https://docs.apebank.io"
          target="_blank"
        >
          <span class="white-0 fz-18">Documentation</span>
        </v-btn>
      </div>

      <div class="mt-10">
        <h1 class="fz-40">What is APEBANK？</h1>
        <div class="mt-5 op-6 fz-16">
          APEBANK is an innovative and optimized product based on $OHM.
          <br />In the V1, we are the same as $OHM (3,3), <br />when APEBANK is
          big, we will launch the V2 (6, 6).
        </div>

        <div class="mt-12">
          <v-btn
            plain
            x-small
            :href="item.href"
            target="_blank"
            class="mr-4"
            v-for="(item, i) in links"
            :key="i"
          >
            <v-icon size="28" color="white">{{ item.icon }}</v-icon>
          </v-btn>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      links: [
        {
          icon: 'mdi-github',
          href: 'https://github.com/apebank',
        },
        {
          icon: 'mdi-twitter',
          href: 'https://twitter.com/apebankdao',
        },
        {
          icon: 'mdi-discord',
          href: 'https://discord.gg/apebank',
        },
      ],
    };
  },
};
</script>
