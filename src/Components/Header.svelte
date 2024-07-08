<script>
  import { goto } from "$app/navigation";

  function navigate() {
    goto("/custom");
  }
</script>

<header class="bg-[#F8F4E1] py-4 rounded-lg mx-auto max-w-md">
  <div class="flex items-center justify-between">
    <h1 class="text-[#543310] text-3xl font-bold">
      Knowledge Representation and Data Analysis
    </h1>
    <button on:click={navigate} class="p-4 pt-2 pb-2 bg-[#AF8F6F] rounded-3xl">Custom Inputs Page</button>
  </div>
</header>