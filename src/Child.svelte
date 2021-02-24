<script>
  import { onMount } from 'svelte';
  import ConfettiGenerator from 'confetti-js';

  onMount(() => {
    const confettiSettings = {
      target: 'my-canvas',
      width: 300,
      height: 100
    };
    const confetti = new ConfettiGenerator(confettiSettings);
    confetti.render();
  });
</script>

<p>this is a child component. confetti:</p>

<canvas id="my-canvas"></canvas>

