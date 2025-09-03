<script>
  const { id = 'input', label, description, error, ...props } = $props();
  const descriptionId = description ? `${id}-description` : undefined;
  const errorId = error ? `${id}-error` : undefined;
</script>

<div class="space-y-1 group">
  <label class="block font-medium text-slate-900 group-has-[input:required]:after:content-['_*'] after:text-red-600" for={id}>{label}</label>
  <input
    class="block outline outline-slate-800 rounded px-2 py-1 focus:outline-2 focus:outline-blue-500 placeholder:italic placeholder-gray-400"
    {id}
    aria-describedby={descriptionId}
    aria-invalid={!!error}
    aria-errormessage={errorId}
    {...props}
  />
  {#if description}
    <p id={descriptionId}>{description}</p>
  {/if}
  {#if error}
    <p id={errorId}>{error}</p>
  {/if}
</div>
