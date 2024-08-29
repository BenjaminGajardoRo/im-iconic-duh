<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Completos ÑAU</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Completos ÑAU</ion-title>
        </ion-toolbar>
      </ion-header>

      <div id="container">
        <strong>¡Bienvenido a ÑAU!</strong>
        <p>Los mejores completos de la ciudad. Elige tu completo favorito y disfruta.</p>
        <ion-button @click="ordenarCompleto">Ordenar Ahora</ion-button>
      </div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { 
  IonContent, 
  IonHeader, 
  IonPage, 
  IonTitle, 
  IonToolbar, 
  IonButton, 
  defineComponent 
} from '@ionic/vue';

const ordenarCompleto = () => {
  console.log("¡Ordena tu completo ahora!");
};
</script>

<style scoped>
#container {
  text-align: center;
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 24px;
  line-height: 32px;
  color: #333;
}

#container p {
  font-size: 18px;
  line-height: 24px;
  color: #555;
  margin: 16px 0;
}

#container ion-button {
  margin-top: 20px;
  --background: #3880ff;
  --background-activated: #3171e0;
}
</style>
