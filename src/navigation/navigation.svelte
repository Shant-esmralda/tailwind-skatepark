{#snippet link(title)}
  <li>
    <a class="px-2 py-5 hover:bg-amber-300" href="#">{title}</a>
  </li>
{/snippet}

<nav class="flex items-center justify-between">
  <a class="bg-gray-900 px-2 py-5 text-white" href="/">Unicorn Corp</a>
  <ul class="flex">
    {@render link('Home')}
    {@render link('About')}
    {@render link('Services')}
    {@render link('Contact')}
  </ul>
</nav>
