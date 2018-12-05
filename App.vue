<template>

  <view class="container">

    <MapView class="container"
    :region="{latitude: 59.21, longitude: 10.41,
    latitudeDelta: 0.3, longitudeDelta: 0.3}">

      <Marker :coordinate="{latitude: 59.21, longitude: 10.41}" />
      <Marker :coordinate="{latitude: 59.17, longitude: 10.45}" />
      <Marker :coordinate="{latitude: 59.18, longitude: 10.43}" />
      <Marker :coordinate="{latitude: 59.20, longitude: 10.40}" />
      <Marker :coordinate="{latitude: 59.15, longitude: 10.39}" />
      <Marker :coordinate="{latitude: 59.25, longitude: 10.39}" />
      <Marker :coordinate="{latitude: 59.24, longitude: 10.40}" />
      <Marker :coordinate="{latitude: 59.10, longitude: 10.42}" />

    </MapView>

    <MapOverlay>

      <HeadingGuide 
        headingText="Hvor skal du?"
      />

      <DestinationBox 
        placeholderText="Posisjon"
      />

    </MapOverlay>

  </view>

</template>

<script>

import MapView  from "react-native-map-clustering";
import { Marker } from "react-native-maps";

import MapOverlay from "./Prompt/MapOverlay.vue";
import HeadingGuide from "./Prompt/HeadingGuide.vue";
import DestinationBox from "./Prompt/DestinationBox.vue";

export default {
   components: {
    MapView,
    Marker,
    MapOverlay,
    HeadingGuide,
    DestinationBox
  }
}

</script>
 
<style>

.container {
  flex: 1;
}

</style>
