<script lang="ts">
  import RecommendedVideos from "$lib/reuseable/RecommendedVideos.svelte";
  import VideoInfo from "$lib/reuseable/VideoInfo.svelte";
  import VideoPlayer from "$lib/reuseable/VideoPlayer.svelte";

  let showMore = false;

</script>

<div class="md:p-7  flex flex-col lg:flex-row gap-7">
  <div  class="w-full">
    <VideoPlayer/>
    <VideoInfo   />
    <div class="p-[21px] mt-[21px] rounded-2xl bg-[#1f2e3c]">
      <p>
        There's something fascinating about vintage charts. Back then they
        believed the information to be so valuable that it should be illustrated
        with incredible detail. I'm glad they did because it inspired me to draw
        this chart based on the Wheel of the Year.
      </p>
      <button
        on:click={() => (showMore = !showMore)}
        class="ml-5 text-[#a2b5c9] font-semibold"
        >Show {showMore ? "less" : "more"}</button
      >
    </div>
  </div>
  <RecommendedVideos />
</div>
