#SP-JobBoard
============

Procedurally generates a job board from pdfs stored in a SharePoint Library

##Usage
============
###Installation
All files must be placed on the same domain as your SharePoint site to avoid errors associated with cross-domain scripting.

###Markup & Initialization
```HTML
<div id="spjobs"></div>

<script type="text/javascript">
  spJobBoard.initModule($('#spjobs'), {guid: 'GUID of SharePoint Document Library goes here!'});
</script>
```

##Variables
-spJobBoard
  - Description: Module namespace.  You must use this variable to configure and initialize the directory module.

##Methods
- initModule
  - Parameters
    - $target : Target DOM element that you wish to call initModule on.
    - options : Object containing the various options you wish to pass to initModule.

##Options
- guid: 
  - Type: String
  - Description: GUID of SharePoint library that you want to make a procedurally generated job board of.

