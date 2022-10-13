<template>
  <ion-page>
    <ion-tabs>
      <ion-router-outlet></ion-router-outlet>
      <ion-tab-bar slot="bottom">
      
        <ion-tab-button tab="tab1" href="/tabs/tab1">
          <ion-icon :icon="libraryOutline" />
          <ion-label>Tab 1</ion-label>
        </ion-tab-button>
          
        <ion-tab-button tab="tab2" href="/tabs/tab2">
          <ion-icon :icon="telescopeOutline" />
          <ion-label>Tab 2</ion-label>
        </ion-tab-button>
        
        <ion-tab-button tab="tab3" href="/tabs/tab3">
          <ion-icon :icon="sparklesOutline" />
          <ion-label>Tab 3</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="tab4" href="/tabs/tab4">
          <ion-icon :icon="sunnyOutline"/>
          <ion-label>Tab 4</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="tab5" href="/tabs/tab5">
          <ion-icon :icon="rocketOutline" />
          <ion-label>Tab 5</ion-label>
        </ion-tab-button>

      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { IonTabBar, IonTabButton, IonTabs, IonLabel, IonIcon, IonPage, IonRouterOutlet } from '@ionic/vue';
import { libraryOutline, sparklesOutline, telescopeOutline, sunnyOutline, rocketOutline } from 'ionicons/icons';

export default defineComponent({
  name: 'TabsPage',
  components: { IonLabel, IonTabs, IonTabBar, IonTabButton, IonIcon, IonPage, IonRouterOutlet },
  setup() {
    return {
      libraryOutline, 
      sparklesOutline, 
      telescopeOutline,
      sunnyOutline,
      rocketOutline
    }
  }
});
</script>
