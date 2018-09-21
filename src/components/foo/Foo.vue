<template>
    <div class="test">
        <h3>Foo</h3>
    </div>
</template>
<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import LatLng = google.maps.LatLng;

@Component
export default class Foo extends Vue {

    private test() {
        const ll = new LatLng(0,0);
        const circle = new google.maps.Circle({
            center: ll,
        });
        circle.getRadius();
    }
}

</script>
