<script>
  import { onDestroy, onMount } from 'svelte';

  const speed = 30;
  const change = 1;

  let logo =
    '<a href="https://reed.kalisz.pl/" alt="logo"><img src="/logo_red.svg" alt="logo" width="50" height="20" /></a>';
  let text = `- pieczątki - ${logo} - tabliczki znamionowe - grawal - ${logo} - automaty samotuszujące - datowniki - ${logo} - tuszownice wymienne - numeratory - ${logo} - Horray - Colop - Trodat - ${logo} - automaty stemplarskie&nbsp;`;

  let content = [text];
  let offsets = [0];

  let widthWindow;
  let widthText;

  let interval;

  onMount(() => {
    interval = setInterval(() => {
      offsets = offsets.map((offset) => offset - change);
      if (offsets[0] < -widthText) {
        content.shift();
        offsets.shift();
      }
      if (offsets[offsets.length - 1] < widthWindow) {
        content.push(text);
        offsets.push(offsets[offsets.length - 1] + widthText);
      }
    }, speed);
  });

  onDestroy(() => {
    clearInterval(interval);
  });
</script>

<svelte:window bind:innerWidth={widthWindow} />

<div class="logo">
  {#each content as text, i}
    <div class="text" bind:offsetWidth={widthText} style={`transform: translate(${offsets[i]}px, -50%)`}>
      {@html text}
    </div>
  {/each}
</div>

<style>
  .logo {
    overflow: hidden;
    position: relative;
    height: 3rem;
    width: 100%;
    background-color: var(--accent);
  }
  .text {
    position: absolute;
    top: 50%;
    left: 0;
    display: flex;
    gap: 1rem;
    white-space: nowrap;
    font-size: 1.1rem;
  }
</style>
