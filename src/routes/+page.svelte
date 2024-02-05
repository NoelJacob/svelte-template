<script lang="ts">
  import Image from '$lib/components/Image.svelte';
  import { Globe } from 'lucide-svelte';
  import { Flame } from 'lucide-svelte';
</script>

<div class="h-screen flex items-center justify-center">
  <Flame size={50} />
  <Image
    src="/favicon.ico"
    width={150}
    height={150}
    alt="The Svelte logo"
    layout="fixed"
    priority={true}
  />
  <Globe size={50} />
</div>

<style lang="postcss">
  div > :global(*) {
    margin: 0;
    padding: 0;
    @apply hover:scale-105 transition-transform;

    &:not(Image) {
      color: #dddddd;
      margin: 0 0.5rem;
    }
  }
</style>
