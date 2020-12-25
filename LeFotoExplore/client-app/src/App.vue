<template>
    <div id="app">
        <div id="map" class="map"></div>
        <div id="info" style="display: none;"></div>
        <label for="track">
            track position
            <input id="track" type="checkbox" />
        </label>
        <p>
            position accuracy : <code id="accuracy"></code>&nbsp;&nbsp;
            altitude : <code id="altitude"></code>&nbsp;&nbsp;
            altitude accuracy : <code id="altitudeAccuracy"></code>&nbsp;&nbsp;
            heading : <code id="heading"></code>&nbsp;&nbsp;
            speed : <code id="speed"></code>
        </p>

    </div>


</template>
<script>
    
</script>
<style >
    .map {
        width: 100%;
        height: 400px;
    }
</style>