<script lang="ts">
  import Image from '$lib/components/Image.svelte';
  import { Globe } from 'lucide-svelte';
  import { Flame } from 'lucide-svelte';
</script>

<div class="h-screen flex items-center justify-center">
  <Flame color="#dddddd" size={50} />
  <Image
    src="/favicon.ico"
    width={150}
    height={150}
    alt="The Svelte logo"
    layout="fixed"
    priority={true}
  />
  <Globe color="#dddddd" size={50} />
</div>

<style lang="postcss">
  div > :global(*) {
    margin: 0;
    padding: 0;
    @apply animate-pulse hover:scale-105 transition-transform;
  }
</style>
