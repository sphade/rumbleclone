<script>
  import Featured from "$lib/reuseable/Featured.svelte";
  import LiveCategory from "$lib/reuseable/LiveCategory.svelte";
  import Sidebar from "$lib/reuseable/Sidebar.svelte";
  import SubHeader from "$lib/reuseable/SubHeader.svelte";
  import VideoSection from "$lib/reuseable/VideoSection.svelte";

</script>

<div class="flex max-w-[1700px] mx-auto w-full ">
  <Sidebar />
  <div class="flex-1 overflow-clip lg:ml-[80px]">
    <SubHeader />
    <Featured />
    <LiveCategory />
    <VideoSection  />
    <!-- <VideoSection /> -->
  </div>
</div>


<style>
  
</style>