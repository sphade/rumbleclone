<script>
  import VideoCard from "./VideoCard.svelte";
</script>

<div class="border-t border-gray-600 px-5 md:px-10 mb-[50px]">
  <div class="mt-[22px] flex justify-between items-center mb-[14px]">
    <h2 class="capitalize text-[22px] font-bold">picks</h2>
    <button
      class="py-[6px] px-[17px] rounded-[140px] font-semibold capitalize transition-colors hover:bg-[#1A2A37] border border-[#85c742]"
      >view all</button
    >
  </div>
  <div
    class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-[24px]"
  >
    {#each { length: 8 } as l}
      <VideoCard />
    {/each}
  </div>
</div>
