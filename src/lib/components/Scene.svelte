<script>
  import { T } from "@threlte/core";
  import { ContactShadows, Grid } from "@threlte/extras";

  import Player from "./Player.svelte";
</script>

<T.DirectionalLight intensity={0.8} position.x={5} position.y={10} />
<T.AmbientLight intensity={0.2} />

<Grid
  position.x={-0.5}
  position.y={-0.5}
  position.z={-0.5}
  cellColor="#ffffff"
  sectionColor="#ffffff"
  sectionThickness={0}
  fadeDistance={30}
  cellSize={1}
/>

<ContactShadows scale={10} blur={2} far={2.5} opacity={0.5} />

<Player />
