<script setup lang="ts">
import {WorkExperience} from "@/components/work/TimelineType";

const timeline: WorkExperience[] = [
  {
    duration: "01-01-2023 - heden",
    company: "myBrand - Geertruidenberg",
    title: "Software Engineer",
    description: "Momenteel werk ik voor myBrand, dit is een bedrijf\n" +
      "gespecialiseerd in SAP integraties. Ik maak deel uit van een Java\n" +
      "team, waarbij we SAP modules uitbreiden door Java applicaties\n" +
      "toe te voegen zodat de SAP modules makkelijker te gebruiken\n" +
      "zijn.\n" +
      "Als onderdeel van mijn taken, heb ik het Spring framework\n" +
      "geïntroduceerd binnen de organisatie, en deze ook toegepast in\n" +
      "een aantal applicaties die in eigen beheer zijn. Verder probeer ik\n" +
      "collega’s te ondersteunen en begeleiden waar nodig.\n" +
      "Naast Spring te introduceren, zijn we ook begonnen met React te\n" +
      "implementeren, de impl",
    color: "primary"
  },
  {
    duration: "01-03-2022 - 31-12-2022",
    company: "Kommaboard - Belgie",
    title: "Software Engineer",
    description: "Bij Kommaboard werkte ik als Java consultant bij DXC. Bij DXC\n" +
      "werk ik als full-stack engineer op 3 verschillende projecten EPC-\n" +
      "FO, EPCNR en Database attesten, het laatste project heb ik\n" +
      "samen met een collega opgezet.\n" +
      "Deze projecten zijn allemaal geschreven in Java. EPCNR en\n" +
      "Database attesten hebben een frontend geschreven met VueJS,\n" +
      "backend van beide projecten is met Java 11 en Maven als build\n" +
      "tool.\n" +
      "EPC-FO gebruikt Java 8 als backend, en als frontend wordt een\n" +
      "combinatie gebruikt van JSP, Wicket en Struts. Maven wordt ook\n" +
      "als build tool gebruikt",
    color: "secondary"
  },
  {
    duration: "01-04-2020 - 28-02-2022",
    company: "Axians - Belgie",
    title: "Junior Software Engineer",
    description: "Voor Axians werk ik aan verschillende projecten. Per project werk\n" +
      "ik met samen met verschillende collega’s. Van de verschillende\n" +
      "projecten heb ik één ‘hoofdproject’ namelijk ‘SKR’. Naast dit\n" +
      "hoofdproject werk ik ook nog aan een aantal ‘kleinere’ projecten.\n" +
      "De meeste applicaties zijn geschreven in een combinatie van\n" +
      "Kotlin, Java en/of Groovy. De frontend is geschreven met VueJS.",
    color: "primary"
  },
  {
    duration: "01-06-2018 - 31-03-2020",
    company: "CZ - Nederland",
    title: "Junior Software Engineer",
    color: "secondary"
  }
]
</script>

<template>
  <v-timeline align="start">
    <v-timeline-item
      v-for="(experience, i) in timeline"
      :key="i"
      :dot-color="experience.color"
      size="small"
    >
      <template v-slot:opposite>
        <div
          :class="`pt-1 headline font-weight-bold text-${experience.color}`"
          v-text="experience.duration"
        ></div>
      </template>
      <div>
        <h2 :class="`mt-n1 headline font-weight-light mb-4 text-${experience.color}`">
          {{ experience.company }}
        </h2>
        <div>
          {{ experience.title }}
        </div>
        <div>{{ experience.description }}</div>
      </div>
    </v-timeline-item>
  </v-timeline>
</template>

<style scoped>

</style>
