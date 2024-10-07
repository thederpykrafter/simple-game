<script>
  import { T } from "@threlte/core";
  import { ContactShadows, Instance, InstancedMesh } from "@threlte/extras";

  import Player from "./Player.svelte";
</script>

<T.DirectionalLight intensity={0.8} position.x={5} position.y={10} />
<T.AmbientLight intensity={0.2} />

<InstancedMesh>
  <T.BoxGeometry />
  <T.MeshStandardMaterial color="#0059BA" />

  {#each { length: 3 } as _, i}
    <Instance position.y={i + 1} />
  {/each}
</InstancedMesh>

<ContactShadows scale={10} blur={2} far={2.5} opacity={0.5} />

<Player />
