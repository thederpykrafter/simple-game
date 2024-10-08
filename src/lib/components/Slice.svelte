<script>
  import { T } from "@threlte/core";
  import { Edges, Instance, InstancedMesh } from "@threlte/extras";
</script>

<InstancedMesh>
  <T.BoxGeometry />
  <T.MeshStandardMaterial color="#0059BA" />

  {#each { length: 3 } as _, i}
    <Instance position.x={i + 1} />
    <Edges color="black" />
  {/each}
</InstancedMesh>
