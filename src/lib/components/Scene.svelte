<script>
  import { T } from "@threlte/core";

  import Player from "./Player.svelte";
  import Slice from "./Slice.svelte";
</script>

<T.DirectionalLight intensity={0.8} position.x={5} position.y={10} />
<T.AmbientLight intensity={0.2} />

<Player />

<Slice />
