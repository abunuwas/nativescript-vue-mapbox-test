<template>
    <Page class="page">
        <ActionBar class="action-bar" title="Vue Mapbox Example"></ActionBar>
        <GridLayout>
                <Mapbox
                    accessToken="the_token"
                    mapStyle="traffic_day"
                    latitude="37.7397"
                    longitude="-121.4252"
                    hideCompass="true"
                    zoomLevel="12"
                    showUserLocation="false"
                    disableZoom="false"
                    disableRotation="false"
                    disableScroll="false"
                    disableTilt="false"
                    @mapReady="onMapReady()">
                </Mapbox>
        </GridLayout>
    </Page>
</template>

<script>
    import * as utils from "utils/utils";
    export default {
        data () {
            return { };
        },
        methods: {
            onMapReady() {
                console.log('map ready')
            }
        }
    };
</script>

<style scoped></style>
