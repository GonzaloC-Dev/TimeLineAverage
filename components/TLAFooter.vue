<template>
  <footer :style="{
    
    width:'100%',
    height:'10%',
    display:'flex',
    flexDirection:'row',
    justifyContent:'center',
    alignItems:'center'
    
  }">
  <div :style="{
    
    width:'40%',
    height:'50%',
    display:'flex',
    justifyContent:'center',
    alignItems:'center',
    flexDirection:'column'
  }">
    <div>Youtube: www.ytbe.com/lineaverage</div>
    <div>Facebook: www.face.com/lineaverage</div>
  </div>
  <div :style="{
    
    width:'40%',
    height:'50%',
    display:'flex',
    justifyContent:'center',
    alignItems:'center',
    flexDirection:'column'
  }">
    <div>Instagram: www.ig.com/lineaverage</div>
    <div>Contact us: 8881(11) 776 344</div>
  </div>
    
  </footer>
</template>

<script>
export default {
  name: "TLAFooter",
};
</script>
