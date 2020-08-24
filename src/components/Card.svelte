<script>
  export let icon;
  export let title;
  export let content;
  export let color1;
  export let color2;
</script>

<div
  class="card rounded rounded-md my-1 mx-3 text-white"
  style=" background: {color1};background: linear-gradient(120deg, {color1} 35%,
  {color2} 100%); ">
  <div class="header flex items-center h-auto w-11/12">
    <div class="icon p-2"><img class="w-8 h-8" src="/icons/{icon}.svg" alt=""></div>
    <div class="title">
       <h1 class="text-2xl font-bold">{title}</h1>
    </div>
  </div>
  <div class="content w-11/12 mx-auto pb-4">{content}</div>
</div>