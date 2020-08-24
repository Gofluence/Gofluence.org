<script>
  import { goto } from "@sapper/app";
  function gotoGithub(event) {
    goto("https://github.com/gofluence/gofluence");
  }
</script>

<div
  class="flex justify-between navbar px-4 py-2 items-center bg-indigo-700 h-24">
  <div class="logo w-1/3 md:w-1/6">
    <img src="/img/logo.svg" alt="Gofluence" />
  </div>
  <div class="comingsoon flex items-center">
    <span class="text-white mr-2">Coming Soon</span>
    <button
      class="hidden md:flex bg-indigo-800 px-2 py-1 rounded text-white text-md"
      on:click={gotoGithub}>
      Interested? Star on Github
    </button>
    <button class="flex md:hidden" on:click={gotoGithub}>
      <svg viewBox="0 0 20 20" fill="currentColor" class="star text-white w-6 h-6">
        <path
          d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0
          00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364
          1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0
          00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0
          00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0
          00.951-.69l1.07-3.292z" />
      </svg>
    </button>
  </div>
</div>
