<script lang="ts">
	import UserMenu from "./UserMenu.svelte";

  let isModalOpen = false;

  function toggleModal() {
    isModalOpen = !isModalOpen;
  }
</script>

<nav class="flex justify-between items-center bg-slate-950 text-slate-100 h-16 ">
  <div>
    <a href="/">Home</a>
    <a href="/about">Friends</a>
    <a href="/contact">Contact</a>
  </div>
  <div>
    <button on:click={toggleModal}>
      <img alt="Default icon for user" src="https://static.vecteezy.com/system/resources/thumbnails/005/129/844/small_2x/profile-user-icon-isolated-on-white-background-eps10-free-vector.jpg" class="rounded-full w-12"/>
    </button>
  </div>
</nav>

<UserMenu isModalOpen={isModalOpen} />
