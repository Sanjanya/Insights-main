<script>
  import Hero from "../Components/Hero.svelte";
  import Description from "../Components/Description.svelte";
  import Insights from "../Components/Insights.svelte";
  import Model from "../Components/Model.svelte";

  function download() {
    const url = "/Knowledge_Representation.ipynb";
    const anchor = document.createElement("a");
    anchor.href = url;
    anchor.setAttribute("download", "Knowledge_Representation.ipynb");
    anchor.click();
  }
  function download_model() {
    const url = "/Models.ipynb";
    const anchor = document.createElement("a");
    anchor.href = url;
    anchor.setAttribute("download", "Models.ipynb");
    anchor.click();
  }
</script>

<main class="flex flex-col">
  <p class="flex text-3xl items-center justify-center font-bold" style="color: #543310">**Heart Disease**</p>
  <Hero />
  <span class="p-8"></span>
  <div class="flex justify-between items-center">
    <h2 class="flex text-3xl ml-6">Ed Analysis and Insight Generation</h2>
    <button
      class="justify-end mr-6 bg-[#AF8F6F] rounded-2xl p-3 pt-2 pb-2"
      on:click={download}
    >
      Download the Colab File</button
    >

  </div>
  <Description />
  <Insights />
  <div class="flex justify-between items-center">
    <h2 class="flex text-3xl ml-6">ML Models</h2>
    <button
      class="justify-end mr-6 bg-[#AF8F6F] rounded-2xl p-3 pt-2 pb-2"
      on:click={download_model}
    >
      Dowload Colab File</button
    >
  </div>
  <Model />
</main>
