<script>
  import Card from "../components/Card.svelte";
  import Typewriter from "typewriter-effect/dist/core";
  import { onMount } from "svelte";
  import Navbar from "../components/Navbar.svelte";
  onMount(() => {
    const typewriter = new Typewriter("#future");
    typewriter
      .typeString("Welcome to Gofluence")
      .pauseFor(10)
      .deleteAll()
      .typeString("The future of livestreaming")
      .start();
  });
</script>

<style>
  .header {
    height: 100vh;
  }
</style>

<svelte:head>
  <title>Gofluence: The Future of Streaming</title>
</svelte:head>
<div class="header">
  <Navbar />
  <div
    class="flex flex-col lg:flex-row my-auto md:pt-12 xl:pt-48 justify-start
    bg-indigo-700">
    <div class="welcome flex-1 text-center">
      <h1
        class="text-2xl md:text-6xl text-gray-100 text-center mb-2"
        id="future" />
      <div class="hidden md:flex md:flex-col">
        <p class="text-gray-100 mx-auto text-md">
          Gofluence is an open source livestreaming platform. That means that
          you run your own server, giving you full control over
          <i>everything.</i>
        </p>
        <p class="text-gray-100 mx-auto text-md">
          Powered by you. Anyone can run their own server, expanding the
          decentralized network.
        </p>
        <p class="text-gray-100 mx-auto text-md">
          Livestreams are peer to peer. This means that once a few viewers have
          started the stream, future viewers will receive the stream via the
          other viewers, reducing bandwidth significantly.
        </p>
      </div>
    </div>
    <div class="cards mx-auto w-full flex-1 flex flex-col">

      <Card
        class="w-full flex-1"
        color1="#fa8231"
        color2="#fd9644"
        icon="decentralized"
        title="Decentralized"
        content="Each instance interconnected with no central servers. Watch any
        livestream on any instance. Peer to peer streaming reduces bandwidth." />

      <Card
        class="w-full flex-1"
        color1="#3867d6"
        color2="#4b7bec"
        icon="private"
        title="Private"
        content="No ads. No invasive trackers. Your data belongs to you. Be in
        full control of your stream." />

      <Card
        class="w-full flex-1"
        color1="#eb3b5a"
        color2="#fc5c65"
        icon="code"
        title="Open Source"
        content="100% of the code powering Gofluence is open source. That means
        anyone can view or edit the code to ensure security." />

    </div>
  </div>
</div>
