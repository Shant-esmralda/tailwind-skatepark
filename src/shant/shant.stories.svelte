<script module>
  import { defineMeta } from '@storybook/addon-svelte-csf';
  import Shant from './shant.svelte';

  const { Story } = defineMeta({
    title: 'Shant',
    component: Shant,
  });
</script>

<Story name="Default" />
