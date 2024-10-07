<script>
  import { T } from "@threlte/core";
  import { OrbitControls, Edges } from "@threlte/extras";
</script>

<T.PerspectiveCamera makeDefault position={[10, 0, 0]} fov={25}>
  <OrbitControls
    enableZoom={true}
    enableDamping
    target.x={0}
    target.y={0}
    target.z={0}
  />
</T.PerspectiveCamera>

<T.Mesh position.x={0} position.y={0} position.z={0}>
  <T.SphereGeometry />
  <T.MeshStandardMaterial color="#0059BA" />
  <Edges color="black" />
</T.Mesh>
