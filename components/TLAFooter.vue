<template>
  <footer
    :style="{
      
      width: '100%',
      height: '10%',
      display: 'flex',
      flexDirection: 'row',
      justifyContent: 'center',
      alignItems: 'center',
    }"
  >
  <div
  :style="{
      backgroundColor: '#000000',
      width: '80%',
      height: '100%',
      display: 'flex',
      flexDirection: 'row',
      justifyContent: 'center',
      alignItems: 'center',
    }">
     <div
      :style="{
        width: '50%',
        height: '50%',
        display: 'flex',
        justifyContent: 'center',
        alignItems: 'center',
        flexDirection: 'column',
      }"
    >
      <div
        :style="{
          color: '#FFFFFF',
        }"
      >
        Youtube: www.ytbe.com/lineaverage
      </div>
      <div
        :style="{
          color: '#FFFFFF',
        }"
      >
        Facebook: www.face.com/lineaverage
      </div>
    </div>
    <div
      :style="{
        width: '50%',
        height: '50%',
        display: 'flex',
        justifyContent: 'center',
        alignItems: 'center',
        flexDirection: 'column',
      }"
    >
      <div
        :style="{
          color: '#FFFFFF',
        }"
      >
        Instagram: www.ig.com/lineaverage
      </div>
      <div
        :style="{
          color: '#FFFFFF',
        }"
      >
        Contact us: 8881(11) 776 344
      </div>
    </div>
  </div>
   
  </footer>
</template>

<script>
export default {
  name: "TLAFooter",
};
</script>
