<template>
  <!-- First father element -->
  <div
    :style="{
      //backgroundColor: 'yellow',
      width: '100%',
      height: '200%',
      display: 'flex',
      justifyContent: 'center',
      flexDirection: 'column',
      alignItems: 'center',
    }"
  >
    <!-- 2 texts father element -->
    <div
      :style="{
        //backgroundColor: 'green',
        width: '80%',
        height: '50%',
      }"
    >
      <div
        :style="{
          //backgroundColor: 'orange',
          width: '100%',
          height: '50%',
          display: 'flex',
          alignItems: 'center',
          justifyContent: 'start',
        }"
      >
        <div
          :style="{
            //backgroundColor: 'purple',
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
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
              reprehenderit in voluptate velit esse cillum dolore eu fugiat
              nulla pariatur.
            </p>
          </div>
        </div>

        <div
          :style="{
            //backgroundColor: 'brown',
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
          //backgroundColor: 'gray',
          width: '100%',
          height: '50%',
          display: 'flex',
          alignItems: 'center',
          justifyContent: 'start',
        }"
      >
        <div
          :style="{
            //backgroundColor: 'brown',
            width: '40%',
            height: '100%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'start',
          }"
        ></div>
        <div
          :style="{
            //backgroundColor: 'red',
            width: '60%',
            height: '100%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'center',
          }"
        >
          <div
            :style="{
              //backgroundColor: 'orange',
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
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat.
            </p>
          </div>
        </div>
      </div>
    </div>
    <!-- Form element -->
    <div
      :style="{
        // backgroundColor: '#F0A332',
        width: '80%',
        height: '50%',
        display: 'flex',
        justifyContent: 'center',
        alignItems: 'center',
      }"
    >
      <div
        :style="{
          //  backgroundColor: 'red',
          width: '90%',
          height: '90%',
          display: 'flex',
          alignItems: 'center',
          flexDirection: 'column',
        }"
      >
        <div
          :style="{
            width: '100%',
            height: '15%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'center',
          }"
        >
          <h1>Envianos tu información de contacto:</h1>
        </div>
        <div
          :style="{
            width: '100%',
            height: '15%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'center',
          }"
        >
          <input
            v-model="FullName"
            class="form-control form-control-lg"
            type="text"
            placeholder="Nombre Completo"
            aria-label=".form-control-lg example"
          />
        </div>
        <div
          :style="{
            width: '100%',
            height: '15%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'center',
          }"
        >
          <input
            v-model="BuisnessName"
            class="form-control form-control-lg"
            type="text"
            placeholder="Nombre de la empresa"
            aria-label=".form-control-lg example"
          />
        </div>
        <div
          :style="{
            width: '100%',
            height: '15%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'center',
          }"
        >
          <input
            v-model="contactEmail"
            class="form-control form-control-lg"
            type="email"
            required
            placeholder="Correo de contacto"
            aria-label=".form-control-lg example"
          />
        </div>
        <div
          :style="{
            width: '100%',
            height: '15%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'center',
          }"
        >
          <input
            v-model="contactTellphone"
            class="form-control form-control-lg"
            type="text"
            placeholder="Télefono de contacto"
            aria-label=".form-control-lg example"
          />
        </div>
        <div
          :style="{
            width: '100%',
            height: '15%',
            display: 'flex',
            alignItems: 'center',
            justifyContent: 'center',
          }"
        >
          <input
            @click="submitForm"
            class="btn btn-primary btn-lg"
            type="submit"
            value="Enviar"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>

//Try use FormElementSize from other file:
//import design from "../assets/componentsSizes/TLAContentSizes"
export default {
  name: "TLAContentPage",
  data: () => ({
    FullName: "",
    BuisnessName: "",
    contactEmail: "",
    contactTellphone: "",
  }),
  methods: {
    submitForm() {
      if (
        this.FullName === "" ||
        this.BuisnessName === "" ||
        this.contactEmail === "" ||
        this.contactTellphone === ""
      ) {
        alert("Verifica los campos");
      } else {
        if (
          this.validateEmail(this.contactEmail)
        ) {
          alert("Se envió con éxito")
          this.emptyAllInput();
        } else {
          //Correct route
          this.emptyInput(this.contactEmail);
          alert("Please enter a valid email address"); 
        }
        
      }
    },
    emptyInput(inputName) {
      return (inputName = "");
    },
    emptyAllInput() {
      this.FullName = "";
      this.BuisnessName = "";
      this.contactEmail = "";
      this.contactTellphone = "";
    },
    validateEmail(email){
      let pattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
      return pattern.test(email);
    }
  },
  
};
</script>
