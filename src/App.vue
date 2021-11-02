<template>
  <ion-app>
    <ion-page>
      <ion-header>
        <ion-toolbar>
          <ion-title> NTC </ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-content>
        <ion-tabs>
          <ion-router-outlet />

          <ion-tab-bar>
            <ion-tab-button tab="Home" href="/home">
              <ion-label>Home</ion-label>
            </ion-tab-button>
            <ion-tab-button tab="Form" href="/form">
              <ion-label>Form</ion-label>
            </ion-tab-button>
            <ion-tab-button tab="Print" href="/print">
              <ion-label>Print</ion-label>
            </ion-tab-button>
          </ion-tab-bar>
        </ion-tabs>
      </ion-content>
    </ion-page>
  </ion-app>
</template>

<script lang="ts">
import {
  IonApp,
  IonRouterOutlet,
  IonPage,
  IonTabs,
  IonTabBar,
  IonTabButton,
  IonLabel,
  IonContent,
  IonHeader,
  IonToolbar,
  IonTitle,
} from "@ionic/vue";
import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
  components: {
    IonApp,
    IonRouterOutlet,
    IonTabs,
    IonTabBar,
    IonTabButton,
    IonLabel,
    IonPage,
    IonContent,
    IonHeader,
    IonToolbar,
    IonTitle,
  },
});
</script>