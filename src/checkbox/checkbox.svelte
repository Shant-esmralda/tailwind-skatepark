<script>
  const { label = 'A Very Important Checkbox', id = 'checkbox', ...props } = $props();
</script>

<div
  class="group rounded border bg-slate-200 p-4 outline-offset-2 outline-sky-400 
  has-checked:border-green-500 has-checked:bg-green-300"
>
  <input type="checkbox" class="peer accent-green-700" {id} {...props}  />
  <label class="group-hover:font-bold peer-checked:line-through peer-checked:text-white" for={id}>{label}</label>
</div>
