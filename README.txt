Qt Design Studio README
=======================

Qt Bridge
---------

Since Qt Design Studio 1.5 the Qt Bridge for Adobe Photoshop and
Qt Bridge for Sketch are not part of the Qt Design Studio package
anymore. License holders can install them by using the Qt online
installer. Licenses can be purchased from the Qt Marketplace.

The Qt online installer copies the Qt Bridge installation packages
to the QtDesignStudio\photoshop_bridge and QtDesignStudio\sketch_bridge
folders in the Qt installation folder.

Since Qt Design Studio 2.1, the Qt Bridge also includes support for Figma.
The Figma plugin can be found in QtDesignStudio\figma_bridge.

The officially supported versions for the Qt Bridges are
Photoshop 22.3.1 and Sketch 72.2.

See the product documentation for more information:
https://doc.qt.io/qtdesignstudio/qtbridge-overview.html

Known Issues in Qt Design Studio 2.1
------------------------------------

- Wizards that do not open files trigger error messages (GridView wizards):
  QDS-241 - Wizards show error message if no file is defined as file to open
- If using webgl streaming (-platform webgl), then
  'QMLSCENE_CORE_PROFILE: "true"' has to be removed from .qmlproject.
- Components like Arc require refreshing the Form Editor if the size is changed.
- Effects are not rendered in Form Editor, unless moved into component
- Effect properties cannot be directly animated. You can  work around this limitation
  by moving the effect into a separate component and binding to a new property defined
  in the root element of the component.
