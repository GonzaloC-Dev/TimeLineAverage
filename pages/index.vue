<template>
  <div
    :style="{
     // backgroundColor: 'yellow',
      width: '100vw',
      height: '100vh',
      minHeight: '100vh'
    }"
  >
    <TLAHeader />
    <TLAContent />
    <TLAFooter />
  </div>
</template>

<script>
export default {
  name: "IndexPage",
};
</script>
