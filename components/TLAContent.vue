<template>
  <div
    :style="{
      // backgroundColor: 'yellow',
      width: '100%',
      height: '80%',
      display: 'flex',
      justifyContent: 'center',
      flexDirection: 'column',
      alignItems: 'center',
    }"
  >
    <div
      :style="{
        // backgroundColor: 'green',
        width: '80%',
        height: '100%',
      }"
    >
      <div
        :style="{
          // backgroundColor: 'orange',
          width: '100%',
          height: '50%',
          display: 'flex',
          alignItems: 'center',
          justifyContent: 'start',
        }"
      >
        <div
          :style="{
            // backgroundColor: 'purple',
            width: '60%',
            height: '100%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'center',
          }"
        >
          <div
            :style="{
              width: '70%',
              height: '30%',
              display: 'flex',
              alignItems: 'center',
              justifyContent: 'center',
              borderLeft: '2px solid #c71818',
            }"
          >
            <p
              :style="{
                textAlign: 'left',
              }"
            >
              The average wait time for lines at banks and cinemas can vary
              greatly depending on the location, time of day, and other factors.
              However, I can provide some general guidelines for estimated wait
              times based on my understanding of common wait times.
            </p>
          </div>
        </div>

        <div
          :style="{
            // backgroundColor: 'brown',
            width: '40%',
            height: '100%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'start',
          }"
        ></div>
      </div>

      <div
        :style="{
          // backgroundColor: 'gray',
          width: '100%',
          height: '50%',
          display: 'flex',
          alignItems: 'center',
          justifyContent: 'start',
        }"
      >
        <div
          :style="{
            // backgroundColor: 'brown',
            width: '40%',
            height: '100%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'start',
          }"
        ></div>
        <div
          :style="{
            // backgroundColor: 'red',
            width: '60%',
            height: '100%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'center',
          }"
        >
          <div
            :style="{
              // backgroundColor: 'orange',
              width: '70%',
              height: '40%',
              display: 'flex',
              alignItems: 'center',
              justifyContent: 'center',
              borderRight: '2px solid #c71818',
            }"
          >
            <p
              :style="{
                textAlign: 'right',
              }"
            >
              The average wait time for lines at banks and cinemas can vary
              greatly depending on the location, time of day, and other factors.
              However, I can provide some general guidelines for estimated wait
              times based on my understanding of common wait times.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TLAContentPage",
};
</script>
