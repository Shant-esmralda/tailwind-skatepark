<script>
  const { title = 'Card Title', description = '' } = $props();
</script>

<div class="border-blue-300 border-2 rounded-sm p-4 bg-blue-50 dark:bg-slate-800 dark:border-slate-600">
  <h2 class="text-4xl font-bold">{title}</h2>
  <p class="mt-4 font-serif">{description}</p>
</div>
