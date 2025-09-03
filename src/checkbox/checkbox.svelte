<script>
  const { label = 'A Very Important Checkbox', id = 'checkbox', ...props } = $props();
</script>

<div
  class="group rounded border flex flex-col gap-2 bg-slate-200 p-4 outline-offset-2
  outline-sky-400 transition-colors has-checked:border-green-500 has-checked:bg-green-300"
>
<div>
  <input type="checkbox" class="peer accent-green-700" {id} {...props} />
  <!-- can do it with group-has-checked:line-through instead of peer -->
  <label class="group-hover:font-bold peer-checked:text-white peer-checked:line-through" for={id}
    >{label}</label
  >
</div>
  <div class=" hidden group-has-checked:block">
    <label>What is the reason?</label>
    <input
      class="block rounded px-2 py-1 placeholder-gray-400 outline outline-slate-800 placeholder:italic focus:outline-2 focus:outline-blue-500"
      placeholder="Enter the reason."
    />
  </div>
</div>
