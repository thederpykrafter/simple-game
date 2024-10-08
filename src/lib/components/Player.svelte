<script>
  import { T } from "@threlte/core";
  import { OrbitControls, Edges } from "@threlte/extras";

  let playerX = 0;
  let playerY = 0;
  let playerZ = 0;
</script>

<T.PerspectiveCamera
  makeDefault
  position={[playerX, playerY, playerZ + 10]}
  fov={35}
>
  <OrbitControls
    enableZoom={true}
    enableDamping
    target.x={playerX}
    target.y={playerY}
    target.z={playerZ}
  />
</T.PerspectiveCamera>

<T.Mesh position.x={playerX} position.y={playerY} position.z={playerZ}>
  <T.SphereGeometry />
  <T.MeshStandardMaterial color="#0059BA" />
  <Edges color="black" />
</T.Mesh>
