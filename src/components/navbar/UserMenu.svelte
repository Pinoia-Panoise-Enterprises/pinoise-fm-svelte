<script lang="ts">
  export let isModalOpen = false;
</script>

<div class={`${isModalOpen ? "block" : "hidden"}`}>
  <div class="absolute right-0 h-fit w-fit px-5 py-4 bg-slate-900 text-slate-100 leading-normal">
    <div class="flex flex-col justify-around"> 
      <a href="/profile">Profile</a>
      <a href="/settings">Settings</a>
      <a href="/settings?tab=connections">Connections</a>
      <a href="/logout">Logout</a>
    </div>
  </div>
</div>