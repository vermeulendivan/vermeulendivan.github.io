---
layout: page
title: Guide
permalink: /guide/
---

# How to extract features
The plugin is user-friendly and extractions can be done as follows:
1. Load a vector line layer to QGIS;
2. Select the layer; and
3. Click on the stream feature extractor icon in the toolbar. The features will be extracted for the selected layer.

![icon](https://github.com/kartoza/stream_feature_extractor/blob/develop/help/source/static/toolbar_icon.png)

4. (optional method) Vector > Stream feature extractor > Extract stream features from current layer.

# Available options
Possible parameters or settings for the plugin can be set. Go to Vector > Stream feature extractor > Options. The following can be set:
1. Search distance: This is the distance used to determine if nodes converged or not. Note: The distance is calculated in map units of your stream network;
2. Show intermediate node count layer: An intermediate layer which were used to extract the feature is loaded to QGIS; and
3. Enabling this will submit errors to the server for debugging.

![options](https://github.com/kartoza/stream_feature_extractor/blob/develop/help/source/static/options_dialog.png)
