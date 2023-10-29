<script lang="ts">
  import { onMount } from "svelte";
  import * as app from "$lib/wailsjs/go/main/App.js";
  let greet: string;
  onMount(async () => {
    greet = await app.Greet("No Name");
  });
</script>

<div class="container h-full mx-auto flex justify-center items-center">
  <div class="space-y-5">
    <h1 class="h1">Let's get cracking bones!</h1>
    <p>Start by exploring: {greet}</p>
    <ul>
      <li>
        <code class="code">/src/routes/+layout.svelte</code> - barebones layout
      </li>
      <li><code class="code">/src/app.postcss</code> - app wide css</li>
      <li>
        <code class="code">/src/routes/+page.svelte</code> - this page, you can replace
        the contents
      </li>
    </ul>
  </div>
</div>
