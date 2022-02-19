<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Users</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true" class="ion-padding">
    <!-- list of text items -->
      <ion-list>
      <ion-list-header>
        <ion-label color="danger">Contact List</ion-label>
      </ion-list-header>
        <ion-item>
          <ion-avatar>
            <img src="../../public/assets/icon/icon.png" alt="">
          </ion-avatar>
          <ion-label>Qwabena</ion-label>
        </ion-item>
        <ion-item>
        <ion-avatar>
            <img src="../../public/assets/icon/icon.png" alt="">
          </ion-avatar>
          <ion-label>Kwabena</ion-label>
        </ion-item>
        <ion-item>
        <ion-avatar>
            <img src="../../public/assets/icon/icon.png" alt="">
          </ion-avatar>
          <ion-label>Olila</ion-label>
        </ion-item>
        <ion-item>
        <ion-avatar>
            <img src="../../public/assets/icon/icon.png" alt="">
          </ion-avatar>
          <ion-label>Akua</ion-label>
        </ion-item>
        <ion-item>
        <ion-avatar>
            <img src="../../public/assets/icon/icon.png" alt="">
          </ion-avatar>
          <ion-label>Abena</ion-label>
        </ion-item>
        <ion-item>
        <ion-avatar>
            <img src="../../public/assets/icon/icon.png" alt="">
          </ion-avatar>
          <ion-label>Kwadwo</ion-label>
        </ion-item>
      </ion-list>

      <!-- list of input items -->
      <ion-list>
        <ion-item>
          <ion-label>Input</ion-label>
          <ion-input></ion-input>
        </ion-item>
        <ion-item>
          <ion-label>Toggle</ion-label>
          <ion-toggle slot="end"></ion-toggle>
        </ion-item>
        <ion-item>
          <ion-label>Radio</ion-label>
          <ion-radio slot="end"></ion-radio>
        </ion-item>
        <ion-item>
          <ion-label>Checkbox</ion-label>
          <ion-checkbox slot="start"></ion-checkbox>
        </ion-item>
      </ion-list>

      <!-- list of sliding Items -->
      <ion-list>
        <ion-item-sliding>
          <ion-item>
          <ion-avatar>
            <img src="../../public/assets/icon/icon.png" alt="">
          </ion-avatar>
            <ion-label>Item</ion-label>
          </ion-item>
          <ion-item-options side="end">
            <ion-item-option @click="unread(item)">Unread</ion-item-option>
          </ion-item-options>
        </ion-item-sliding>
      </ion-list>

    </ion-content>
  </ion-page>
</template>

<script lang="ts">
  import { 
    IonCheckbox,
    IonInput,
    IonItem,
    IonItemOption,
    IonItemOptions,
    IonItemSliding,
    IonListHeader,
    IonAvatar,
    IonList,
    IonLabel, 
    IonRadio,
    IonToggle,
    IonContent, 
    IonHeader, 
    IonPage, 
    IonTitle, 
    IonToolbar 
  } from '@ionic/vue';
  import { defineComponent } from 'vue';

  export default defineComponent({
    name: 'Tab1Page',
    components: {
      IonCheckbox,
      IonInput,
      IonItem,
      IonItemOption,
      IonItemOptions,
      IonItemSliding,
      IonListHeader,
      IonAvatar,
      IonList,
      IonLabel, 
      IonRadio,
      IonToggle,
      IonContent, 
      IonHeader, 
      IonPage, 
      IonTitle, 
      IonToolbar 
    },
  });
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
    font-size: 20px;
    line-height: 26px;
  }

  #container p {
    font-size: 16px;
    line-height: 22px;

    color: #8c8c8c;

    margin: 0;
  }

  #container a {
    text-decoration: none;
  }
</style>