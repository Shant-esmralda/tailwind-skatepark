<script>
  const { label = 'A Very Important Checkbox', id = 'checkbox', ...props } = $props();
</script>

<div class="rounded border bg-slate-200 p-4 outline-offset-2 outline-sky-400 focus-within:bg-sky-200">
  <input class="peer accent-purple-300" {id} {...props} type="checkbox" />
  <label class="peer-checked:line-through" for={id}>{label}</label>
</div>
