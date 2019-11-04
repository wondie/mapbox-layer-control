# mapbox-layer-control

#### [Grouped Demo](https://reyemtm.github.io/mapbox-layer-control/example/grouped.html) experimental

#### [Simple Demo](https://reyemtm.github.io/mapbox-layer-control/example/simple.html)

*This is very much in development and may change without notice.*

This is a simple layer control for Mapbox GL JS maps inspired by the Gartrell Group legend control. The layers need to already exist in the map. Each layer should only be added once to the control. The control does not control map layer indexing. The layers should be added to the control in the opposite order that they have been added to the map. The control simply adjusts the visibility layout property of the layer. In the grouped control, the group name toggles all the layers in the group. The control can have hidden layers that get toggled just like other layers. Layers have legends added automatically if they are a line, circle or fill with a single color. They can also have legend written in HTML.

To Do:

* [ ] ADD DOCUMENTATION

* [ ] ADD TOGGLE ICON, COLLAPSIBLE ICON AND COLLAPSIBLE METHOD TO GROUP HEADING FOR HIDDEN LAYERS
* [?] ACCESSIBILITY FOR HIDDEN LAYERS, LAYER HEADINGS AND DIRECTORY HEADINGS???
* [ ] FIX WEIRD SELECTION BUG WHEN CLICK HEADING AND MOUSEOUT
* [ ] FIX HOVER/COLLAPSED EFFECT ON MOBILE
* [-] ADD CSS FRAMEWORK STYLING FOR TOGGLES
* [X] STYLE COLLAPSIBLE GROUP HEADINGS WITH HEIGHT TRANSITIONS
* [X] MOVE STYLES TO STYLESHEET
* [X] DECIDE ON LEGEND PLACEMENT VS HIDDEN LAYER PLACEMENT
* [x] ADD HIDDEN LAYERS
* [x] ADD LEGEND ITEMS
* [x] ADD COLLAPSIBLE DIRECTORY HEADINGS

![](simple.jpg)

```javascript
map.addControl( new layerControlSimple({
  layers: ["Lakes", "States", "Counties"]
}), "top-left");
```
Data is from [Natural Earth](https://www.naturalearthdata.com/) and [here](https://eric.clst.org/tech/usgeojson/).
