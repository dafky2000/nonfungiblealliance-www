<template lang="html">
  <div>
    <a 
      id="partners" 
      name="partners" 
      class="anchor"/>
    <div class="partners grid-container">
      <h2>{{ title }}</h2>
      <div class="logos grid-x align-center grid-margin-x grid-margin-y">
        <div 
          v-for="item in items.slice(0, limit)" 
          :key="item.id" 
          class="logo small-6 medium-4 large-3 cell align-self-middle">
          <img :src="`/partners/${item}`">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      default: 'Recently joined',
      type: String
    },
    limit: {
      default: 16,
      type: Number
    }
  },
  data() {
    return {
      items: [
        'block-base.svg',
        'blockade-games.png',
        'blockchain-slovakia.png',
        'coin-kred.svg',
        'crypto-baseball.png',
        'crypto-space-commander.png',
        'dcl-plazas.png',
        'lucid-sight.png',
        'neon-district.png',
        'nft-nyc.svg',
        'unik-name.png',
        'artchain.png',
        'bitski.png',
        'cryptage-origins.png',
        'crypto-motors.png',
        'cryptographics.png',
        'dapp-radar.png',
        'decenter.png',
        'encrypted.jpg',
        'hyperbridge.png',
        'mintable.png',
        'phantasma.png',
        'pixura.png',
        'po8.png',
        'streamers-connected.png',
        'trade-stars.png',
        'wetrust.png',
        'bloch.png',
        'block3.png',
        'blockchaingamernet.png',
        'coingecko.png',
        'covalent.png',
        'crypto-kaiju.png',
        'cryptobeasties.png',
        'cryptocrystal.png',
        'cubego.png',
        'd0x.png',
        'decentralanddaily.png',
        'divino.png',
        'ecomi.png',
        'ether-kingdom.jpg',
        'etheremon.png',
        'farsight-podcast.png',
        'horizon.png',
        'iba.png',
        'invented4.png',
        'kauku.png',
        'larva-labs.svg',
        'lumi-collect.png',
        'matic.png',
        'minting-coins.png',
        'nifty-gateway.png',
        'verified-collection.png',
        'aave.png',
        'auctionity.png',
        'demystify.png',
        'fuel-games.png',
        'gods-unchained.png',
        '0xgame.png',
        'sorare.png',
        'trg.jpg',
        'vault.png',
        'webp.png',
        'hyperdragons.png',
        'block-rocket.png',
        'blockchain-studios.png',
        'codex.png',
        'hashmark.png',
        'crypto-carz.png',
        'crypto-decks.png',
        'dac.png',
        'dapp.png',
        'ember-sword.png',
        'eth-town.png',
        'kette.png',
        'known-origin.png',
        'mokens.png',
        'non-fungible.png',
        'opensea.png',
        'su-squares.png',
        'unico.png',
        'doctrina.svg',
        'tokntok.svg',
        'socouch.png',
        '0xcert.svg'
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.partners {
  padding: 2rem 1rem;

  img {
    max-height: 80px;
  }

  h2 {
    margin: 0 auto;
    text-align: center;
  }

  .logos {
    margin: 2rem 0;
  }

  .logo {
    box-shadow: $box-shadow-light;
    padding: 1rem 2rem;
    border-radius: 5px;
    border: 1px solid rgba(125, 130, 133, 0.05);
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 130px;
  }
}
</style>
