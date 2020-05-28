<template>
  <p class="player-rank">
    Global Rank: <span style="color:#fac244"> #{{ user.rank }}</span>
  </p>
</template>

<script lang="ts">
  import { UserData } from '@/types/common-types';
  import { Component, Vue, Mixins, Prop } from 'vue-property-decorator';
  @Component({})
  export default class PlayerHeader extends Vue {
    @Prop() user!: UserData;
  }
</script>
