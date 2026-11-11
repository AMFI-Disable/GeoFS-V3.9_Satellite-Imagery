# Changelog

All notable changes, photorealistic satellite imagery pipelines, and version releases for GeoFS-V3.9 Satellite Imagery are documented in this file.

---

## [3.9.0] - Unified Metadata

### Changed

- Standardize the userscript metadata and version across the V3.9 ecosystem.
- Match only the GeoFS main site and activate only when it reports V3.9.

---

## [1.1.5] - GeoFS V3.9 Compatibility

### Changed

- Start only after GeoFS reports V3.9; remain inactive on other or unrecognized versions.
- Update compatibility documentation and version metadata.

---

## [1.1.4] - Esri Tile Initialization Fix

### Changed

- Replaced the failing Esri metadata-based provider with direct Cesium tile requests.
- Displayed a warning if imagery tiles cannot load.
- Initialize imagery even when GeoFS already reports HD mode.

---

## [1.1.3] - Esri World Imagery

### Changed

- **Esri World Imagery**: Replaced the Bing aerial provider with Esri World Imagery.
- **Attribution**: Added Esri and imagery provider credits to the Cesium imagery layer.
- **Metadata**: Updated the script description and startup notification for this release.

---

## [1.1.0] - Stable Bing Aerial HD Background Engine

### Added

- **Bing Aerial HD Engine**: Promoted Bing Aerial HD engine to stable release.
- **Robust Initialization Lifecycle**: Implemented 10-second initialization delay ensuring GeoFS core services, Cesium viewer, and deferred assets finish loading before imagery injection.
- **Bing Maps Imagery Provider**: Direct binding with `Cesium.BingMapsImageryProvider` for full global ultra-resolution photorealistic satellite coverage.
- **Elevation Mesh Shading**: Integrated `FlatRunwayTerrainProvider` and SRTM elevation meshes with vertex normal shading.

### Changed

- **Distraction-Free Zero UI**: Completely removed all on-screen control panels and widgets for zero UI interference.
- **Notification Toast**: Standardized startup notification with `V39_NOTIF.success`.

---

## [1.0.4] - Bing Aerial HD And Zero-UI Streamlining

### Changed

- **Exclusive Bing Aerial Provider**: Streamlined the satellite imagery engine to exclusively use Bing Aerial Ultra-Resolution imagery and SRTM HD terrain elevation meshes.
- **Distraction-Free Cockpit**: Completely eliminated on-screen panels and manual selectors for a clean cockpit experience.

---

## [1.0.0] - Initial Production Release

### Added

- **Dynamic Imagery Swapping**: Dynamic in-memory Cesium imagery provider swapping without page reloads.
- **High-Resolution Provider Support**: Support for Google Satellite, Apple Maps Satellite, and Bing Aerial providers.
- **HD Terrain Support**: Enabled HD terrain elevation support with SRTM elevation data.
- **AdSense Suppression**: Built-in automatic AdSense container removal for an ad-free simulation experience.
