<script>
  import { T } from "@threlte/core";
  import { OrbitControls } from "@threlte/extras";
</script>

<T.PerspectiveCamera makeDefault position={[-10, 10, 10]} fov={15}>
  <OrbitControls
    enableZoom={true}
    enableDamping
    target.x={0}
    target.y={0}
    target.z={0}
  />
</T.PerspectiveCamera>

<T.Mesh position.x={0} position.y={0} position.z={0}>
  <T.BoxGeometry />
  <T.MeshStandardMaterial color="#0059BA" />
</T.Mesh>
