# Comparing `tmp/qsharp_widgets-1.3.5.dev0-py2.py3-none-any.whl.zip` & `tmp/qsharp_widgets-1.3.6.dev0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 149662 bytes, number of entries: 6
+Zip file size: 150194 bytes, number of entries: 6
 -rw-r--r--  2.0 unx     7449 b- defN 20-Feb-02 00:00 qsharp_widgets/__init__.py
--rw-r--r--  2.0 unx    12054 b- defN 20-Feb-02 00:00 qsharp_widgets/static/index.css
--rw-r--r--  2.0 unx   484290 b- defN 20-Feb-02 00:00 qsharp_widgets/static/index.js
-?rw-r--r--  2.0 unx      192 b- defN 20-Feb-02 00:00 qsharp_widgets-1.3.5.dev0.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 qsharp_widgets-1.3.5.dev0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      503 b- defN 20-Feb-02 00:00 qsharp_widgets-1.3.5.dev0.dist-info/RECORD
-6 files, 504593 bytes uncompressed, 148756 bytes compressed:  70.5%
+-rw-r--r--  2.0 unx    12066 b- defN 20-Feb-02 00:00 qsharp_widgets/static/index.css
+-rw-r--r--  2.0 unx   485694 b- defN 20-Feb-02 00:00 qsharp_widgets/static/index.js
+?rw-r--r--  2.0 unx      192 b- defN 20-Feb-02 00:00 qsharp_widgets-1.3.6.dev0.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 qsharp_widgets-1.3.6.dev0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      503 b- defN 20-Feb-02 00:00 qsharp_widgets-1.3.6.dev0.dist-info/RECORD
+6 files, 506009 bytes uncompressed, 149288 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: qsharp_widgets/static/index.css
 Comment: 
 
 Filename: qsharp_widgets/static/index.js
 Comment: 
 
-Filename: qsharp_widgets-1.3.5.dev0.dist-info/METADATA
+Filename: qsharp_widgets-1.3.6.dev0.dist-info/METADATA
 Comment: 
 
-Filename: qsharp_widgets-1.3.5.dev0.dist-info/WHEEL
+Filename: qsharp_widgets-1.3.6.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: qsharp_widgets-1.3.5.dev0.dist-info/RECORD
+Filename: qsharp_widgets-1.3.6.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qsharp_widgets/static/index.css

```diff
@@ -1 +1 @@
-:root{--heading-background: #262679;--main-background: var( --vscode-editor-background, var(--jp-layout-color0, #ececf0) );--main-color: var( --vscode-editor-foreground, var(--jp-widgets-color, #202020) );--qs-tr-nth-color: var( --vscode-list-hoverBackground, var(--jp-layout-color1, var(--colab-secondary-surface-color, #f2f2f2)) );--nav-background: #bed1f4;--nav-hover-background: #b3bede;--nav-current-background: #b5c5f2;--border-color: #768f9c;--menu-box-fill: var(--main-background);--error-background-color: #ffe3e3;--bar-selected-outline: #587ddd}*,*:before,*:after{box-sizing:inherit;margin:0;padding:0}html{box-sizing:border-box;font-size:16px}.qs-play-body{position:relative;min-height:100vh;font-family:system-ui,Segoe UI,SegoeUI,Roboto,Helvetica,Arial,sans-serif;color:var(--main-color);background-color:var(--main-background);display:grid;grid-template-areas:"header header header" "nav editor results";grid-template-rows:auto 1fr;grid-template-columns:minmax(180px,auto) 8fr 8fr;column-gap:16px}.page-header{grid-area:header;background:var(--heading-background);color:var(--main-background);font-size:2rem;font-weight:600;text-align:center;padding-top:4px;padding-bottom:8px}#popup{position:absolute;display:none;background-color:#fff;border:1px solid black;border-radius:2px;padding:8px 16px;font-size:16px}.nav-column{grid-area:nav;background-color:var(--nav-background)}.nav-1{font-size:1.2rem;font-weight:200;color:var(--main-color);border-top:1px solid var(--border-color);padding-top:4px;padding-bottom:4px;padding-left:8px}.nav-2{font-size:1rem;font-weight:200;padding:4px 4px 4px 16px}.nav-selectable:hover{background-color:var(--nav-hover-background);cursor:pointer}.nav-current{font-weight:700;background-color:var(--nav-current-background)}.editor-column{grid-area:editor;margin:32px 16px 16px}.file-name{border:1px solid var(--border-color);border-bottom:0px;width:100px;text-align:center;height:32px;line-height:32px;background-color:#fff}.icon-row>*{margin-left:4px;font-size:1.4rem;cursor:pointer}.code-editor{height:40vh;min-height:400px;border:1px solid var(--border-color)}.button-row{display:flex;justify-content:flex-end;align-items:center;margin-top:8px}.button-row>*{margin-left:10px;font-size:1rem}.main-button{background-color:var(--nav-background);font-size:1rem;color:var(--main-color);width:72px;height:24px;border-radius:8px;border:1px solid var(--border-color);cursor:pointer}.main-button:disabled{background-color:gray;cursor:default}.error-list{margin-top:24px;margin-bottom:24px;min-height:48px}.error-row{border:1px solid var(--border-color);background-color:var(--error-background-color);padding:4px;border-bottom:.5px solid gray;font-size:.9rem;margin-bottom:-1px}.error-row>span{font-weight:200}.error-help{font-weight:200;font-style:italic}.kata-override{background-color:var(--main-background)}.results-column{grid-area:results;margin-left:0;margin-top:32px;margin-right:120px}.active-tab{font-size:1.1rem;font-weight:600;text-decoration:underline}.results-labels{display:flex;height:32px}.results-labels>div{margin-right:40px;text-align:left;vertical-align:middle;cursor:pointer}.hir-output{height:40vh;min-height:400px;width:100%;resize:none;white-space:pre}.output-header{font-size:1.1rem;font-weight:400;margin-top:16px;margin-bottom:16px;display:flex;justify-content:space-between}.prev-next{font-weight:200;cursor:pointer}.result-label{margin-bottom:24px;font-style:italic;font-weight:300}.message-output{font-weight:300;font-size:1.1rem;margin-bottom:16px}.state-table{border-collapse:collapse;font-size:.9rem;width:100%;min-width:400px;margin-bottom:16px}.state-table thead tr{background:var(--nav-background)}.state-table tbody tr{border-top:1px solid gray}.state-table td,.state-table th{text-align:center;padding:6px;white-space:nowrap}.state-table progress{margin-right:2px}.histogram{max-height:calc(100vh - 40px);max-width:600px;border:1px solid var(--border-color);background-color:var(--vscode-sideBar-background, white)}.bar{fill:var(--vscode-button-background, var(--nav-background))}.bar:hover{fill:var(--vscode-button-hoverBackground, var(--nav-hover-background))}.bar-selected{stroke:var(--bar-selected-outline);fill:var(--nav-current-background)}.bar-label{font-size:3pt;fill:var(--vscode-button-foreground, var(--main-color));text-anchor:end;pointer-events:none}.histo-label{font-size:3.5pt;fill:var(--vscode-foreground, #3b3b3b)}.hover-text{font-size:3.5pt;fill:gray;text-anchor:middle}.menu-icon *{stroke:#000;fill:var(--vscode-sideBar-background, white);stroke:var(--vscode-icon-foreground, #3b3b3b)}.menu-box{fill:var(--menu-box-fill);stroke:#000;stroke-width:.1}.menu-item{width:32px;height:10px;fill:var(--vscode-list-inactiveSelectionBackground, var(--nav-background));stroke:gray;stroke-width:.2}.menu-item:hover{stroke-width:.6;fill:var(--vscode-list-hoverBackground, var(--nav-hover-background))}.menu-selected{fill:var( --vscode-list-activeSelectionBackground, var(--nav-current-background) )}.menu-text{font-size:4.5px;pointer-events:none;fill:var(--main-color)}.menu-separator{stroke:gray;stroke-width:.25}.help-info{fill:var(--menu-box-fill);stroke:gray;stroke-width:.5}.help-info-text{font-size:4.5px;pointer-events:none;fill:var(--main-color)}.estimate-details{padding:1em}.estimate-details>summary{font-size:1.1em}.estimate-table{margin-top:1em;font-size:.9em}.estimate-table tr:nth-child(2n){background-color:var(--qs-tr-nth-color)}.estimate-cell{vertical-align:top;padding-right:8px}.title-cell{font-weight:700;white-space:nowrap}.value-cell{text-align:center;width:100px;white-space:nowrap}.estimate-explanation{margin-top:1em;margin-bottom:1em;max-width:500px}.estimate-assumption{margin:1em}.cell-output-ipywidget-background{background-color:transparent!important}#pieChart{fill:var(--main-color)}.spaceReport{display:flex;flex-direction:column}.spaceReportHeader{font-size:13px;background-color:var(--qs-tr-nth-color);border-top:.5px gray solid;border-bottom:.5px gray solid;padding:10px}.spaceReportRow{display:flex;font-size:12px;padding:10px 24px}.spaceDetailText{width:200px}.qs-help{font-size:14px;line-height:1.5;word-wrap:break-word}.qs-help h1{margin-top:16px;margin-bottom:8px;line-height:1.25;font-weight:600;padding-bottom:.3em;font-size:2em;border-bottom:1px solid var(--vscode-editorWidget-border)}.qs-help h2{margin-top:16px;margin-bottom:8px;font-weight:600;line-height:1.25;padding-bottom:.3em;font-size:1.4em;border-bottom:1px solid var(--vscode-editorWidget-border)}.qs-resultsTable-sortedTable{border-collapse:collapse;margin:12px 0;outline:none}.qs-resultsTable-sortedTable th,.qs-resultsTable-sortedTable td{padding:4px 8px;text-align:left}.qs-resultsTable-dragEnter{background-color:#8888;border-left:1.5px solid blue;border-right:1.5px solid blue}.qs-resultsTable-sortedTable tr:nth-child(2n){background:var(--qs-tr-nth-color)}.qs-resultsTable-sortedTable tbody tr:hover{background:var(--vscode-list-hoverBackground, var(--js-layout-color2))}.qs-resultsTable-sortedTableSelectedRow td{background:var(--vscode-button-background, var(--jp-layout-color3));color:var(--vscode-button-foreground);font-weight:600}.qs-resultsTable-columnMenu{display:none;width:160px}.qs-resultsTable-showColumnMenu{display:block;position:absolute;background-color:var(--vscode-menu-background, var(--main-background));border:1px solid #8888;padding:4px;z-index:100;text-align:left}.qs-resultsTable-menuItem{cursor:pointer;background-color:var(--vscode-list-hoverBackground, var(--jp-layout-color1));padding:4px;margin:2px;font-size:14px;font-weight:400}.qs-resultsTable-menuItem:hover{background-color:var(--vscode-menu-border, var(--jp-layout-color2))}.qs-resultsTable-columnSelected{cursor:pointer;padding:4px;font-weight:400;font-size:14px;background-color:var(--vscode-button-background, var(--jp-brand-color1));color:var(--vscode-button-foreground, var(--jp-ui-inverse-font-color0));margin:2px;border-radius:3px}.qs-resultsTable-headerCell{padding-right:20px}.qs-resultsTable-sortHeaderCell{padding-right:4px}@keyframes codicon-spin{to{transform:rotate(360deg);transform-origin:center}}.codicon-modifier-spin{fill:var(--vscode-icon-foreground, gray);animation:codicon-spin 1.5s steps(45) infinite}.qs-scatterChart-x-axisTitle,.qs-scatterChart-y-axisTitle{text-anchor:middle;font-size:16px;fill:var(--main-color)}.qs-scatterChart-y-axisTitle{writing-mode:vertical-lr;transform:rotate(180deg)}.qs-scatterChart-point{r:2px;stroke-width:4px}.qs-scatterChart-hover:hover{r:4px;stroke-width:4px;fill:#fff}.qs-scatterChart-point-selected{r:8px;stroke-width:4px;fill:#fff}.qs-scatterChart-watermark{font-size:16px;fill:var(--main-color)}.qs-scatterChart-tooltip,.qs-scatterChart-selectedInfo{position:absolute;visibility:hidden;background:var(--main-background);color:var(--main-color);border:var(--border-color) 1px solid;padding:4px}.qs-scatterChart-tooltip:after,.qs-scatterChart-selectedInfo:after{content:"";position:absolute;bottom:100%;left:50%;margin-left:-5px;border-width:5px;border-style:solid;border-color:transparent transparent var(--border-color) transparent}.qs-scatterChart-axis,.qs-scatterChart-tick-line{stroke:var(--border-color)}.qs-scatterChart-x-tick-text{text-anchor:middle;fill:var(--main-color)}.qs-scatterChart-y-tick-text{text-anchor:end;fill:var(--main-color)}.qs-estimatesOverview-error{color:red}.qs-circuit-panel p,.qs-circuit-error,.qs-circuit-error p{padding:10px 0}.qs-circuit{background:var(--main-background)}.qs-circuit line,.qs-circuit circle,.qs-circuit rect{stroke:var(--main-color);stroke-width:1}.qs-circuit text{fill:var(--main-color);dominant-baseline:middle;text-anchor:middle;font-family:Arial}.qs-circuit .gate-unitary{fill:var(--vscode-button-secondaryBackground, #d9f1fa)}.qs-circuit .gate text{fill:var(--vscode-button-secondaryForeground, #000000)}.qs-circuit .gate>line,.qs-circuit .control-dot{fill:var(--main-color)}.qs-circuit .gate>.oplus>line,.qs-circuit .gate>.oplus>circle{fill:var(--main-background);stroke:var(--main-color);stroke-width:2}.qs-circuit .gate-measure{fill:var(--vscode-button-background, #ffde86)}.qs-circuit .gate>g>line,.qs-circuit .arc-measure{stroke:var(--vscode-button-foreground, #000000);fill:none;stroke-width:1}.qs-circuit rect.gate-swap{fill:transparent;stroke:transparent}.qs-circuit .register-classical{stroke-width:.5}.qs-circuit .hidden{display:none}.qs-circuit .classically-controlled-unknown{opacity:.25}.qs-circuit .classically-controlled-one .classical-container,.qs-circuit .classically-controlled-one .classical-line{stroke:#4059bd;stroke-width:1.3;fill:#4059bd;fill-opacity:.1}.qs-circuit .classically-controlled-zero .classical-container,.qs-circuit .classically-controlled-zero .classical-line{stroke:#c40000;stroke-width:1.3;fill:#c40000;fill-opacity:.1}.qs-circuit .classically-controlled-btn{cursor:pointer}.qs-circuit .classically-controlled-unknown .classically-controlled-btn{fill:#e5e5e5}.qs-circuit .classically-controlled-one .classically-controlled-btn{fill:#4059bd}.qs-circuit .classically-controlled-zero .classically-controlled-btn{fill:#c40000}.qs-circuit .classically-controlled-btn text{dominant-baseline:middle;text-anchor:middle;stroke:none;font-family:Arial}.qs-circuit .classically-controlled-unknown .classically-controlled-btn text{fill:#000}.qs-circuit .classically-controlled-one .classically-controlled-btn text{fill:#fff}.qs-circuit .classically-controlled-zero .classically-controlled-btn text{fill:#fff}.qs-circuit .qviz .gate-collapse,.qs-circuit .qviz .gate-expand{opacity:0;transition:opacity 1s}.qs-circuit .qviz:hover .gate-collapse,.qs-circuit .qviz:hover .gate-expand{visibility:visible;opacity:.2;transition:visibility 1s;transition:opacity 1s}.qs-circuit .gate-expand,.gate-collapse{cursor:pointer}.qs-circuit .gate-collapse circle,.qs-circuit .gate-expand circle{fill:#fff;stroke-width:2px;stroke:#000}.qs-circuit .gate-collapse path,.qs-circuit .gate-expand path{stroke-width:4px;stroke:#000}.qs-circuit .gate:hover>.gate-collapse,.qs-circuit .gate:hover>.gate-expand{visibility:visible;opacity:1;transition:opacity 1s}
+:root{--heading-background: #262679;--main-background: var( --vscode-editor-background, var(--jp-layout-color0, #ececf0) );--main-color: var( --vscode-editor-foreground, var(--jp-widgets-color, #202020) );--qs-tr-nth-color: var( --vscode-list-hoverBackground, var(--jp-layout-color1, var(--colab-secondary-surface-color, #f2f2f2)) );--nav-background: #bed1f4;--nav-hover-background: #b3bede;--nav-current-background: #b5c5f2;--border-color: #768f9c;--menu-box-fill: var(--main-background);--error-background-color: #ffe3e3;--bar-selected-outline: #587ddd}*,*:before,*:after{box-sizing:inherit;margin:0;padding:0}html{box-sizing:border-box;font-size:16px}.qs-play-body{position:relative;min-height:100vh;font-family:system-ui,Segoe UI,SegoeUI,Roboto,Helvetica,Arial,sans-serif;color:var(--main-color);background-color:var(--main-background);display:grid;grid-template-areas:"header header header" "nav editor results";grid-template-rows:auto 1fr;grid-template-columns:minmax(180px,auto) 8fr 8fr;column-gap:16px}.page-header{grid-area:header;background:var(--heading-background);color:var(--main-background);font-size:2rem;font-weight:600;text-align:center;padding-top:4px;padding-bottom:8px}#popup{position:absolute;display:none;background-color:#fff;border:1px solid black;border-radius:2px;padding:8px 16px;font-size:16px}.nav-column{grid-area:nav;background-color:var(--nav-background)}.nav-1{font-size:1.2rem;font-weight:200;color:var(--main-color);border-top:1px solid var(--border-color);padding-top:4px;padding-bottom:4px;padding-left:8px}.nav-2{font-size:1rem;font-weight:200;padding:4px 4px 4px 16px}.nav-selectable:hover{background-color:var(--nav-hover-background);cursor:pointer}.nav-current{font-weight:700;background-color:var(--nav-current-background)}.editor-column{grid-area:editor;margin:32px 16px 16px}.file-name{border:1px solid var(--border-color);border-bottom:0px;width:100px;text-align:center;height:32px;line-height:32px;background-color:#fff}.icon-row>*{margin-left:4px;font-size:1.4rem;cursor:pointer}.code-editor{height:40vh;min-height:400px;border:1px solid var(--border-color)}.button-row{display:flex;justify-content:flex-end;align-items:center;margin-top:8px}.button-row>*{margin-left:10px;font-size:1rem}.main-button{background-color:var(--nav-background);font-size:1rem;color:var(--main-color);width:72px;height:24px;border-radius:8px;border:1px solid var(--border-color);cursor:pointer}.main-button:disabled{background-color:gray;cursor:default}.error-list{margin-top:24px;margin-bottom:24px;min-height:48px}.error-row{border:1px solid var(--border-color);background-color:var(--error-background-color);padding:4px;border-bottom:.5px solid gray;font-size:.9rem;margin-bottom:-1px}.error-row>span{font-weight:200}.error-help{font-weight:200;font-style:italic}.kata-override{background-color:var(--main-background)}.results-column{grid-area:results;margin-left:0;margin-top:32px;margin-right:120px}.active-tab{font-size:1.1rem;font-weight:600;text-decoration:underline}.results-labels{display:flex;height:32px}.results-labels>div{margin-right:40px;text-align:left;vertical-align:middle;cursor:pointer}.ast-output,.hir-output{height:40vh;min-height:400px;width:100%;resize:none;white-space:pre}.output-header{font-size:1.1rem;font-weight:400;margin-top:16px;margin-bottom:16px;display:flex;justify-content:space-between}.prev-next{font-weight:200;cursor:pointer}.result-label{margin-bottom:24px;font-style:italic;font-weight:300}.message-output{font-weight:300;font-size:1.1rem;margin-bottom:16px}.state-table{border-collapse:collapse;font-size:.9rem;width:100%;min-width:400px;margin-bottom:16px}.state-table thead tr{background:var(--nav-background)}.state-table tbody tr{border-top:1px solid gray}.state-table td,.state-table th{text-align:center;padding:6px;white-space:nowrap}.state-table progress{margin-right:2px}.histogram{max-height:calc(100vh - 40px);max-width:600px;border:1px solid var(--border-color);background-color:var(--vscode-sideBar-background, white)}.bar{fill:var(--vscode-button-background, var(--nav-background))}.bar:hover{fill:var(--vscode-button-hoverBackground, var(--nav-hover-background))}.bar-selected{stroke:var(--bar-selected-outline);fill:var(--nav-current-background)}.bar-label{font-size:3pt;fill:var(--vscode-button-foreground, var(--main-color));text-anchor:end;pointer-events:none}.histo-label{font-size:3.5pt;fill:var(--vscode-foreground, #3b3b3b)}.hover-text{font-size:3.5pt;fill:gray;text-anchor:middle}.menu-icon *{stroke:#000;fill:var(--vscode-sideBar-background, white);stroke:var(--vscode-icon-foreground, #3b3b3b)}.menu-box{fill:var(--menu-box-fill);stroke:#000;stroke-width:.1}.menu-item{width:32px;height:10px;fill:var(--vscode-list-inactiveSelectionBackground, var(--nav-background));stroke:gray;stroke-width:.2}.menu-item:hover{stroke-width:.6;fill:var(--vscode-list-hoverBackground, var(--nav-hover-background))}.menu-selected{fill:var( --vscode-list-activeSelectionBackground, var(--nav-current-background) )}.menu-text{font-size:4.5px;pointer-events:none;fill:var(--main-color)}.menu-separator{stroke:gray;stroke-width:.25}.help-info{fill:var(--menu-box-fill);stroke:gray;stroke-width:.5}.help-info-text{font-size:4.5px;pointer-events:none;fill:var(--main-color)}.estimate-details{padding:1em}.estimate-details>summary{font-size:1.1em}.estimate-table{margin-top:1em;font-size:.9em}.estimate-table tr:nth-child(2n){background-color:var(--qs-tr-nth-color)}.estimate-cell{vertical-align:top;padding-right:8px}.title-cell{font-weight:700;white-space:nowrap}.value-cell{text-align:center;width:100px;white-space:nowrap}.estimate-explanation{margin-top:1em;margin-bottom:1em;max-width:500px}.estimate-assumption{margin:1em}.cell-output-ipywidget-background{background-color:transparent!important}#pieChart{fill:var(--main-color)}.spaceReport{display:flex;flex-direction:column}.spaceReportHeader{font-size:13px;background-color:var(--qs-tr-nth-color);border-top:.5px gray solid;border-bottom:.5px gray solid;padding:10px}.spaceReportRow{display:flex;font-size:12px;padding:10px 24px}.spaceDetailText{width:200px}.qs-help{font-size:14px;line-height:1.5;word-wrap:break-word}.qs-help h1{margin-top:16px;margin-bottom:8px;line-height:1.25;font-weight:600;padding-bottom:.3em;font-size:2em;border-bottom:1px solid var(--vscode-editorWidget-border)}.qs-help h2{margin-top:16px;margin-bottom:8px;font-weight:600;line-height:1.25;padding-bottom:.3em;font-size:1.4em;border-bottom:1px solid var(--vscode-editorWidget-border)}.qs-resultsTable-sortedTable{border-collapse:collapse;margin:12px 0;outline:none}.qs-resultsTable-sortedTable th,.qs-resultsTable-sortedTable td{padding:4px 8px;text-align:left}.qs-resultsTable-dragEnter{background-color:#8888;border-left:1.5px solid blue;border-right:1.5px solid blue}.qs-resultsTable-sortedTable tr:nth-child(2n){background:var(--qs-tr-nth-color)}.qs-resultsTable-sortedTable tbody tr:hover{background:var(--vscode-list-hoverBackground, var(--js-layout-color2))}.qs-resultsTable-sortedTableSelectedRow td{background:var(--vscode-button-background, var(--jp-layout-color3));color:var(--vscode-button-foreground);font-weight:600}.qs-resultsTable-columnMenu{display:none;width:160px}.qs-resultsTable-showColumnMenu{display:block;position:absolute;background-color:var(--vscode-menu-background, var(--main-background));border:1px solid #8888;padding:4px;z-index:100;text-align:left}.qs-resultsTable-menuItem{cursor:pointer;background-color:var(--vscode-list-hoverBackground, var(--jp-layout-color1));padding:4px;margin:2px;font-size:14px;font-weight:400}.qs-resultsTable-menuItem:hover{background-color:var(--vscode-menu-border, var(--jp-layout-color2))}.qs-resultsTable-columnSelected{cursor:pointer;padding:4px;font-weight:400;font-size:14px;background-color:var(--vscode-button-background, var(--jp-brand-color1));color:var(--vscode-button-foreground, var(--jp-ui-inverse-font-color0));margin:2px;border-radius:3px}.qs-resultsTable-headerCell{padding-right:20px}.qs-resultsTable-sortHeaderCell{padding-right:4px}@keyframes codicon-spin{to{transform:rotate(360deg);transform-origin:center}}.codicon-modifier-spin{fill:var(--vscode-icon-foreground, gray);animation:codicon-spin 1.5s steps(45) infinite}.qs-scatterChart-x-axisTitle,.qs-scatterChart-y-axisTitle{text-anchor:middle;font-size:16px;fill:var(--main-color)}.qs-scatterChart-y-axisTitle{writing-mode:vertical-lr;transform:rotate(180deg)}.qs-scatterChart-point{r:2px;stroke-width:4px}.qs-scatterChart-hover:hover{r:4px;stroke-width:4px;fill:#fff}.qs-scatterChart-point-selected{r:8px;stroke-width:4px;fill:#fff}.qs-scatterChart-watermark{font-size:16px;fill:var(--main-color)}.qs-scatterChart-tooltip,.qs-scatterChart-selectedInfo{position:absolute;visibility:hidden;background:var(--main-background);color:var(--main-color);border:var(--border-color) 1px solid;padding:4px}.qs-scatterChart-tooltip:after,.qs-scatterChart-selectedInfo:after{content:"";position:absolute;bottom:100%;left:50%;margin-left:-5px;border-width:5px;border-style:solid;border-color:transparent transparent var(--border-color) transparent}.qs-scatterChart-axis,.qs-scatterChart-tick-line{stroke:var(--border-color)}.qs-scatterChart-x-tick-text{text-anchor:middle;fill:var(--main-color)}.qs-scatterChart-y-tick-text{text-anchor:end;fill:var(--main-color)}.qs-estimatesOverview-error{color:red}.qs-circuit-panel p,.qs-circuit-error,.qs-circuit-error p{padding:10px 0}.qs-circuit{background:var(--main-background)}.qs-circuit line,.qs-circuit circle,.qs-circuit rect{stroke:var(--main-color);stroke-width:1}.qs-circuit text{fill:var(--main-color);dominant-baseline:middle;text-anchor:middle;font-family:Arial}.qs-circuit .gate-unitary{fill:var(--vscode-button-secondaryBackground, #d9f1fa)}.qs-circuit .gate text{fill:var(--vscode-button-secondaryForeground, #000000)}.qs-circuit .gate>line,.qs-circuit .control-dot{fill:var(--main-color)}.qs-circuit .gate>.oplus>line,.qs-circuit .gate>.oplus>circle{fill:var(--main-background);stroke:var(--main-color);stroke-width:2}.qs-circuit .gate-measure{fill:var(--vscode-button-background, #ffde86)}.qs-circuit .gate>g>line,.qs-circuit .arc-measure{stroke:var(--vscode-button-foreground, #000000);fill:none;stroke-width:1}.qs-circuit rect.gate-swap{fill:transparent;stroke:transparent}.qs-circuit .register-classical{stroke-width:.5}.qs-circuit .hidden{display:none}.qs-circuit .classically-controlled-unknown{opacity:.25}.qs-circuit .classically-controlled-one .classical-container,.qs-circuit .classically-controlled-one .classical-line{stroke:#4059bd;stroke-width:1.3;fill:#4059bd;fill-opacity:.1}.qs-circuit .classically-controlled-zero .classical-container,.qs-circuit .classically-controlled-zero .classical-line{stroke:#c40000;stroke-width:1.3;fill:#c40000;fill-opacity:.1}.qs-circuit .classically-controlled-btn{cursor:pointer}.qs-circuit .classically-controlled-unknown .classically-controlled-btn{fill:#e5e5e5}.qs-circuit .classically-controlled-one .classically-controlled-btn{fill:#4059bd}.qs-circuit .classically-controlled-zero .classically-controlled-btn{fill:#c40000}.qs-circuit .classically-controlled-btn text{dominant-baseline:middle;text-anchor:middle;stroke:none;font-family:Arial}.qs-circuit .classically-controlled-unknown .classically-controlled-btn text{fill:#000}.qs-circuit .classically-controlled-one .classically-controlled-btn text{fill:#fff}.qs-circuit .classically-controlled-zero .classically-controlled-btn text{fill:#fff}.qs-circuit .qviz .gate-collapse,.qs-circuit .qviz .gate-expand{opacity:0;transition:opacity 1s}.qs-circuit .qviz:hover .gate-collapse,.qs-circuit .qviz:hover .gate-expand{visibility:visible;opacity:.2;transition:visibility 1s;transition:opacity 1s}.qs-circuit .gate-expand,.gate-collapse{cursor:pointer}.qs-circuit .gate-collapse circle,.qs-circuit .gate-expand circle{fill:#fff;stroke-width:2px;stroke:#000}.qs-circuit .gate-collapse path,.qs-circuit .gate-expand path{stroke-width:4px;stroke:#000}.qs-circuit .gate:hover>.gate-collapse,.qs-circuit .gate:hover>.gate-expand{visibility:visible;opacity:1;transition:opacity 1s}
```

## qsharp_widgets/static/index.js

### js-beautify {}

```diff
@@ -1,40 +1,40 @@
-var th = Object.create;
-var Ko = Object.defineProperty;
-var rh = Object.getOwnPropertyDescriptor;
-var nh = Object.getOwnPropertyNames;
-var ih = Object.getPrototypeOf,
-    oh = Object.prototype.hasOwnProperty;
+var rh = Object.create;
+var na = Object.defineProperty;
+var nh = Object.getOwnPropertyDescriptor;
+var ih = Object.getOwnPropertyNames;
+var oh = Object.getPrototypeOf,
+    ah = Object.prototype.hasOwnProperty;
 var W = (r, e) => () => (e || r((e = {
     exports: {}
 }).exports, e), e.exports);
-var ah = (r, e, i, a) => {
+var sh = (r, e, i, a) => {
     if (e && typeof e == "object" || typeof e == "function")
-        for (let l of nh(e)) !oh.call(r, l) && l !== i && Ko(r, l, {
+        for (let l of ih(e)) !ah.call(r, l) && l !== i && na(r, l, {
             get: () => e[l],
-            enumerable: !(a = rh(e, l)) || a.enumerable
+            enumerable: !(a = nh(e, l)) || a.enumerable
         });
     return r
 };
-var qn = (r, e, i) => (i = r != null ? th(ih(r)) : {}, ah(e || !r || !r.__esModule ? Ko(i, "default", {
+var Mn = (r, e, i) => (i = r != null ? rh(oh(r)) : {}, sh(e || !r || !r.__esModule ? na(i, "default", {
     value: r,
     enumerable: !0
 }) : i, r));
-var On = W(Dr => {
+var $n = W(Dr => {
     "use strict";
     Object.defineProperty(Dr, "__esModule", {
         value: !0
     });
     Dr.RegisterType = void 0;
-    var Fh;
+    var Bh;
     (function(r) {
         r[r.Qubit = 0] = "Qubit", r[r.Classical = 1] = "Classical"
-    })(Fh = Dr.RegisterType || (Dr.RegisterType = {}))
+    })(Bh = Dr.RegisterType || (Dr.RegisterType = {}))
 });
-var Ut = W(me => {
+var Wt = W(me => {
     "use strict";
     Object.defineProperty(me, "__esModule", {
         value: !0
     });
     me.regLineStart = me.argsFontSize = me.labelFontSize = me.controlBtnRadius = me.controlBtnOffset = me.nestedGroupPadding = me.groupBoxPadding = me.classicalRegHeight = me.registerHeight = me.labelPadding = me.gatePadding = me.gateHeight = me.minGateWidth = me.startY = me.startX = me.leftPadding = me.svgNS = void 0;
     me.svgNS = "http://www.w3.org/2000/svg";
     me.leftPadding = 20;
@@ -50,885 +50,885 @@
     me.nestedGroupPadding = 2;
     me.controlBtnOffset = 40;
     me.controlBtnRadius = 15;
     me.labelFontSize = 14;
     me.argsFontSize = 12;
     me.regLineStart = 40
 });
-var b0 = W(_e => {
+var y0 = W(_e => {
     "use strict";
     Object.defineProperty(_e, "__esModule", {
         value: !0
     });
     _e.dashedBox = _e.dashedLine = _e.arc = _e.text = _e.box = _e.controlDot = _e.circle = _e.line = _e.group = _e.createSvgElement = void 0;
-    var Ba = Ut(),
-        Bh = function(r, e) {
+    var Ia = Wt(),
+        Nh = function(r, e) {
             e === void 0 && (e = {});
-            var i = document.createElementNS(Ba.svgNS, r);
+            var i = document.createElementNS(Ia.svgNS, r);
             return Object.entries(e).forEach(function(a) {
                 var l = a[0],
                     c = a[1];
                 return i.setAttribute(l, c)
             }), i
         };
-    _e.createSvgElement = Bh;
-    var Nh = function(r, e) {
+    _e.createSvgElement = Nh;
+    var Lh = function(r, e) {
         e === void 0 && (e = {});
         var i = (0, _e.createSvgElement)("g", e);
         return r.forEach(function(a) {
             return i.appendChild(a)
         }), i
     };
-    _e.group = Nh;
-    var Lh = function(r, e, i, a, l) {
+    _e.group = Lh;
+    var Ph = function(r, e, i, a, l) {
         var c = {
             x1: r.toString(),
             x2: i.toString(),
             y1: e.toString(),
             y2: a.toString()
         };
         return l != null && (c.class = l), (0, _e.createSvgElement)("line", c)
     };
-    _e.line = Lh;
-    var Ph = function(r, e, i, a) {
+    _e.line = Ph;
+    var Ih = function(r, e, i, a) {
         var l = {
             cx: r.toString(),
             cy: e.toString(),
             r: i.toString()
         };
         return a != null && (l.class = a), (0, _e.createSvgElement)("circle", l)
     };
-    _e.circle = Ph;
-    var Ih = function(r, e, i) {
+    _e.circle = Ih;
+    var Oh = function(r, e, i) {
         return i === void 0 && (i = 5), (0, _e.circle)(r, e, i, "control-dot")
     };
-    _e.controlDot = Ih;
-    var Oh = function(r, e, i, a, l) {
+    _e.controlDot = Oh;
+    var Hh = function(r, e, i, a, l) {
         return l === void 0 && (l = "gate-unitary"), (0, _e.createSvgElement)("rect", {
             class: l,
             x: r.toString(),
             y: e.toString(),
             width: i.toString(),
             height: a.toString()
         })
     };
-    _e.box = Oh;
-    var Hh = function(r, e, i, a) {
-        a === void 0 && (a = Ba.labelFontSize);
+    _e.box = Hh;
+    var $h = function(r, e, i, a) {
+        a === void 0 && (a = Ia.labelFontSize);
         var l = (0, _e.createSvgElement)("text", {
             "font-size": a.toString(),
             x: e.toString(),
             y: i.toString()
         });
         return l.textContent = r, l
     };
-    _e.text = Hh;
-    var $h = function(r, e, i, a) {
+    _e.text = $h;
+    var Gh = function(r, e, i, a) {
         return (0, _e.createSvgElement)("path", {
             class: "arc-measure",
             d: "M ".concat(r + 2 * i, " ").concat(e, " A ").concat(i, " ").concat(a, " 0 0 0 ").concat(r, " ").concat(e)
         })
     };
-    _e.arc = $h;
-    var Gh = function(r, e, i, a, l) {
+    _e.arc = Gh;
+    var Vh = function(r, e, i, a, l) {
         var c = (0, _e.line)(r, e, i, a, l);
         return c.setAttribute("stroke-dasharray", "8, 8"), c
     };
-    _e.dashedLine = Gh;
-    var Vh = function(r, e, i, a, l) {
+    _e.dashedLine = Vh;
+    var jh = function(r, e, i, a, l) {
         var c = (0, _e.box)(r, e, i, a, l);
         return c.setAttribute("fill-opacity", "0"), c.setAttribute("stroke-dasharray", "8, 8"), c
     };
-    _e.dashedBox = Vh
+    _e.dashedBox = jh
 });
-var Ia = W(ur => {
+var Ga = W(ur => {
     "use strict";
     Object.defineProperty(ur, "__esModule", {
         value: !0
     });
     ur._qubitInput = ur.formatInputs = void 0;
-    var Na = On(),
-        zr = Ut(),
-        La = b0(),
-        jh = function(r) {
+    var Oa = $n(),
+        zr = Wt(),
+        Ha = y0(),
+        Uh = function(r) {
             var e = [],
                 i = {},
                 a = zr.startY;
             return r.forEach(function(l) {
                 var c = l.id,
                     d = l.numChildren;
-                if (e.push(Pa(a)), i[c] = {
-                        type: Na.RegisterType.Qubit,
+                if (e.push($a(a)), i[c] = {
+                        type: Oa.RegisterType.Qubit,
                         y: a
                     }, d == null || d === 0) {
                     a += zr.registerHeight;
                     return
                 }
                 a += zr.classicalRegHeight, i[c].children = Array.from(Array(d), function() {
-                    var m = {
-                        type: Na.RegisterType.Classical,
+                    var f = {
+                        type: Oa.RegisterType.Classical,
                         y: a
                     };
-                    return a += zr.classicalRegHeight, m
+                    return a += zr.classicalRegHeight, f
                 })
             }), {
-                qubitWires: (0, La.group)(e),
+                qubitWires: (0, Ha.group)(e),
                 registers: i,
                 svgHeight: a
             }
         };
-    ur.formatInputs = jh;
-    var Pa = function(r) {
-        var e = (0, La.text)("|0\u27E9", zr.leftPadding, r, 16);
+    ur.formatInputs = Uh;
+    var $a = function(r) {
+        var e = (0, Ha.text)("|0\u27E9", zr.leftPadding, r, 16);
         return e.setAttribute("text-anchor", "start"), e.setAttribute("dominant-baseline", "middle"), e
     };
-    ur._qubitInput = Pa
+    ur._qubitInput = $a
 });
 var hr = W(Rr => {
     "use strict";
     Object.defineProperty(Rr, "__esModule", {
         value: !0
     });
     Rr.GateType = void 0;
-    var Uh;
+    var Wh;
     (function(r) {
         r[r.Measure = 0] = "Measure", r[r.Cnot = 1] = "Cnot", r[r.Swap = 2] = "Swap", r[r.X = 3] = "X", r[r.Unitary = 4] = "Unitary", r[r.ControlledUnitary = 5] = "ControlledUnitary", r[r.ClassicalControlled = 6] = "ClassicalControlled", r[r.Group = 7] = "Group", r[r.Invalid = 8] = "Invalid"
-    })(Uh = Rr.GateType || (Rr.GateType = {}))
+    })(Wh = Rr.GateType || (Rr.GateType = {}))
 });
-var Ya = W(Le => {
+var Ja = W(Le => {
     "use strict";
     var Nt = Le && Le.__spreadArray || function(r, e, i) {
         if (i || arguments.length === 2)
             for (var a = 0, l = e.length, c; a < l; a++)(c || !(a in e)) && (c || (c = Array.prototype.slice.call(e, 0, a)), c[a] = e[a]);
         return r.concat(c || Array.prototype.slice.call(e))
     };
     Object.defineProperty(Le, "__esModule", {
         value: !0
     });
     Le._classicalControlled = Le._groupedOperations = Le._controlledGate = Le._swap = Le._unitary = Le._measure = Le._zoomButton = Le._createGate = Le._formatGate = Le.formatGates = void 0;
     var gt = hr(),
-        Re = Ut(),
-        be = b0(),
-        y0 = function(r, e) {
+        Re = Wt(),
+        be = y0(),
+        x0 = function(r, e) {
             e === void 0 && (e = 0);
             var i = r.map(function(a) {
-                return Oa(a, e)
+                return Va(a, e)
             });
             return (0, be.group)(i)
         };
-    Le.formatGates = y0;
-    var Oa = function(r, e) {
+    Le.formatGates = x0;
+    var Va = function(r, e) {
         e === void 0 && (e = 0);
         var i = r.type,
             a = r.x,
             l = r.controlsY,
             c = r.targetsY,
             d = r.label,
-            m = r.displayArgs,
+            f = r.displayArgs,
             g = r.width;
         switch (i) {
             case gt.GateType.Measure:
-                return rr([$a(a, l[0])], r, e);
+                return nr([Ua(a, l[0])], r, e);
             case gt.GateType.Unitary:
-                return rr([Gn(d, a, c, g, m)], r, e);
+                return nr([jn(d, a, c, g, f)], r, e);
             case gt.GateType.X:
-                return rr([Yh(r, e)], r, e);
+                return nr([Zh(r, e)], r, e);
             case gt.GateType.Swap:
-                return l.length > 0 ? Hn(r, e) : rr([Ga(r, e)], r, e);
+                return l.length > 0 ? Gn(r, e) : nr([Wa(r, e)], r, e);
             case gt.GateType.Cnot:
             case gt.GateType.ControlledUnitary:
-                return Hn(r, e);
+                return Gn(r, e);
             case gt.GateType.Group:
-                return Ua(r, e);
+                return Qa(r, e);
             case gt.GateType.ClassicalControlled:
-                return Wa(r);
+                return Xa(r);
             default:
                 throw new Error("ERROR: unknown gate (".concat(d, ") of type ").concat(i, "."))
         }
     };
-    Le._formatGate = Oa;
-    var rr = function(r, e, i) {
+    Le._formatGate = Va;
+    var nr = function(r, e, i) {
         var a = (e || {}).dataAttributes,
             l = {
                 class: "gate"
             };
         Object.entries(a || {}).forEach(function(d) {
-            var m = d[0],
+            var f = d[0],
                 g = d[1];
-            return l["data-".concat(m)] = g
+            return l["data-".concat(f)] = g
         });
-        var c = Ha(e, i);
+        var c = ja(e, i);
         return c != null && (r = r.concat([c])), (0, be.group)(r, l)
     };
-    Le._createGate = rr;
-    var Ha = function(r, e) {
+    Le._createGate = nr;
+    var ja = function(r, e) {
         if (r == null) return null;
-        var i = $n(r, e),
+        var i = Vn(r, e),
             a = i[0],
             l = i[1],
             c = r.dataAttributes;
         c = c || {};
         var d = "expanded" in c,
-            m = a + 2,
+            f = a + 2,
             g = l + 2,
-            y = (0, be.circle)(m, g, 10);
+            y = (0, be.circle)(f, g, 10);
         if (d) {
             var _ = (0, be.createSvgElement)("path", {
-                    d: "M".concat(m - 7, ",").concat(g, " h14")
+                    d: "M".concat(f - 7, ",").concat(g, " h14")
                 }),
-                k = [y, _];
-            return (0, be.group)(k, {
+                w = [y, _];
+            return (0, be.group)(w, {
                 class: "gate-control gate-collapse"
             })
         } else if (c["zoom-in"] == "true") {
             var T = (0, be.createSvgElement)("path", {
-                    d: "M".concat(m, ",").concat(g - 7, " v14 M").concat(m - 7, ",").concat(g, " h14")
+                    d: "M".concat(f, ",").concat(g - 7, " v14 M").concat(f - 7, ",").concat(g, " h14")
                 }),
-                k = [y, T];
-            return (0, be.group)(k, {
+                w = [y, T];
+            return (0, be.group)(w, {
                 class: "gate-control gate-expand"
             })
         }
         return null
     };
-    Le._zoomButton = Ha;
-    var $n = function(r, e) {
+    Le._zoomButton = ja;
+    var Vn = function(r, e) {
             var i = r.x,
                 a = r.width,
                 l = r.type,
                 c = r.targetsY,
                 d = c?.flatMap(function(L) {
                     return L
                 }) || [],
-                m = Math.max.apply(Math, d),
+                f = Math.max.apply(Math, d),
                 g = Math.min.apply(Math, d),
-                y, _, k, T;
+                y, _, w, T;
             switch (l) {
                 case gt.GateType.Group:
                     var A = Re.groupBoxPadding - e * Re.nestedGroupPadding;
-                    return y = i - 2 * A, _ = g - Re.gateHeight / 2 - A, k = a + 2 * A, T = m + +Re.gateHeight / 2 + A - (g - Re.gateHeight / 2 - A), [y, _, k, T];
+                    return y = i - 2 * A, _ = g - Re.gateHeight / 2 - A, w = a + 2 * A, T = f + +Re.gateHeight / 2 + A - (g - Re.gateHeight / 2 - A), [y, _, w, T];
                 default:
-                    y = i - a / 2, _ = g - Re.gateHeight / 2, k = i + a, T = m + Re.gateHeight / 2
+                    y = i - a / 2, _ = g - Re.gateHeight / 2, w = i + a, T = f + Re.gateHeight / 2
             }
-            return [y, _, k, T]
+            return [y, _, w, T]
         },
-        $a = function(r, e) {
+        Ua = function(r, e) {
             r -= Re.minGateWidth / 2;
             var i = Re.minGateWidth,
                 a = Re.gateHeight,
                 l = (0, be.box)(r, e - a / 2, i, a, "gate-measure"),
                 c = (0, be.arc)(r + 5, e + 2, i / 2 - 5, a / 2 - 8),
                 d = (0, be.line)(r + i / 2, e + 8, r + i - 8, e - a / 2 + 8);
             return (0, be.group)([l, c, d])
         };
-    Le._measure = $a;
-    var Gn = function(r, e, i, a, l, c) {
+    Le._measure = Ua;
+    var jn = function(r, e, i, a, l, c) {
         if (c === void 0 && (c = !0), i.length === 0) throw new Error("Failed to render unitary gate (".concat(r, "): has no y-values"));
         var d = i.map(function(T) {
             var A = T[T.length - 1],
                 L = T[0],
                 R = A - L + Re.gateHeight;
-            return Wh(r, e, L, a, R, l)
+            return Yh(r, e, L, a, R, l)
         });
         if (c && d.length > 1) {
-            var m = i[i.length - 1],
+            var f = i[i.length - 1],
                 g = i[0],
-                y = m[m.length - 1],
+                y = f[f.length - 1],
                 _ = g[0],
-                k = (0, be.dashedLine)(e, _, e, y);
-            return (0, be.group)(Nt([k], d, !0))
+                w = (0, be.dashedLine)(e, _, e, y);
+            return (0, be.group)(Nt([w], d, !0))
         }
         return (0, be.group)(d)
     };
-    Le._unitary = Gn;
-    var Wh = function(r, e, i, a, l, c) {
+    Le._unitary = jn;
+    var Yh = function(r, e, i, a, l, c) {
             l === void 0 && (l = Re.gateHeight), i -= Re.gateHeight / 2;
             var d = (0, be.box)(e - a / 2, i, a, l),
-                m = i + l / 2 - (c == null ? 0 : 7),
-                g = (0, be.text)(r, e, m),
+                f = i + l / 2 - (c == null ? 0 : 7),
+                g = (0, be.text)(r, e, f),
                 y = [d, g];
             if (c != null) {
                 var _ = i + l / 2 + 8,
-                    k = (0, be.text)(c, e, _, Re.argsFontSize);
-                y.push(k)
+                    w = (0, be.text)(c, e, _, Re.argsFontSize);
+                y.push(w)
             }
             return (0, be.group)(y)
         },
-        Ga = function(r, e) {
+        Wa = function(r, e) {
             var i = r.x,
                 a = r.targetsY,
-                l = $n(r, e),
+                l = Vn(r, e),
                 c = l[0],
                 d = l[1],
-                m = l[2],
+                f = l[2],
                 g = l[3],
                 y = a?.flatMap(function(A) {
                     return A
                 }) || [],
-                _ = (0, be.box)(c, d, m, g, "gate-swap"),
-                k = y.map(function(A) {
-                    return Va(i, A)
+                _ = (0, be.box)(c, d, f, g, "gate-swap"),
+                w = y.map(function(A) {
+                    return Ya(i, A)
                 }),
                 T = (0, be.line)(i, y[0], i, y[1]);
-            return (0, be.group)(Nt(Nt([_], k, !0), [T], !1))
+            return (0, be.group)(Nt(Nt([_], w, !0), [T], !1))
         };
-    Le._swap = Ga;
-    var Yh = function(r, e) {
+    Le._swap = Wa;
+    var Zh = function(r, e) {
             var i = r.x,
                 a = r.targetsY,
                 l = a.flatMap(function(c) {
                     return c
                 });
-            return ja(i, l[0])
+            return Za(i, l[0])
         },
-        Va = function(r, e) {
+        Ya = function(r, e) {
             var i = 8,
                 a = (0, be.line)(r - i, e - i, r + i, e + i),
                 l = (0, be.line)(r - i, e + i, r + i, e - i);
             return (0, be.group)([a, l])
         },
-        Hn = function(r, e) {
+        Gn = function(r, e) {
             var i = [],
                 a = r.type,
                 l = r.x,
                 c = r.controlsY,
                 d = r.label,
-                m = r.displayArgs,
+                f = r.displayArgs,
                 g = r.width,
                 y = r.targetsY;
             switch (a) {
                 case gt.GateType.Cnot:
-                    y.forEach(function(G) {
-                        return i.push(ja(l, G))
+                    y.forEach(function(O) {
+                        return i.push(Za(l, O))
                     });
                     break;
                 case gt.GateType.Swap:
-                    y.forEach(function(G) {
-                        return i.push(Va(l, G))
+                    y.forEach(function(O) {
+                        return i.push(Ya(l, O))
                     });
                     break;
                 case gt.GateType.ControlledUnitary:
                     var _ = y;
-                    i.push(Gn(d, l, _, g, m, !1)), y = y.flat();
+                    i.push(jn(d, l, _, g, f, !1)), y = y.flat();
                     break;
                 default:
                     throw new Error("ERROR: Unrecognized gate: ".concat(d, " of type ").concat(a))
             }
-            var k = c.map(function(G) {
-                    return (0, be.controlDot)(l, G)
+            var w = c.map(function(O) {
+                    return (0, be.controlDot)(l, O)
                 }),
                 T = Math.max.apply(Math, Nt(Nt([], c, !1), y, !1)),
                 A = Math.min.apply(Math, Nt(Nt([], c, !1), y, !1)),
                 L = (0, be.line)(l, A, l, T),
-                R = rr(Nt(Nt([L], k, !0), i, !0), r, e);
+                R = nr(Nt(Nt([L], w, !0), i, !0), r, e);
             return R
         };
-    Le._controlledGate = Hn;
-    var ja = function(r, e, i) {
+    Le._controlledGate = Gn;
+    var Za = function(r, e, i) {
             i === void 0 && (i = 15);
             var a = (0, be.circle)(r, e, i),
                 l = (0, be.line)(r, e - i, r, e + i),
                 c = (0, be.line)(r - i, e, r + i, e);
             return (0, be.group)([a, l, c], {
                 class: "oplus"
             })
         },
-        Ua = function(r, e) {
+        Qa = function(r, e) {
             var i = r.children,
-                a = $n(r, e),
+                a = Vn(r, e),
                 l = a[0],
                 c = a[1],
                 d = a[2],
-                m = a[3],
-                g = (0, be.dashedBox)(l, c, d, m),
+                f = a[3],
+                g = (0, be.dashedBox)(l, c, d, f),
                 y = [g];
-            return i != null && y.push(y0(i, e + 1)), rr(y, r, e)
+            return i != null && y.push(x0(i, e + 1)), nr(y, r, e)
         };
-    Le._groupedOperations = Ua;
-    var Wa = function(r, e) {
+    Le._groupedOperations = Qa;
+    var Xa = function(r, e) {
         e === void 0 && (e = Re.groupBoxPadding);
         var i = r.controlsY,
             a = r.dataAttributes,
             l = r.targetsY,
             c = r.children,
             d = r.x,
-            m = r.width,
+            f = r.width,
             g = i[0],
             y = [];
         if (c != null) {
             if (c.length !== 2) throw new Error("Invalid number of children found for classically-controlled gate: ".concat(c.length));
-            var _ = y0(c[0]);
+            var _ = x0(c[0]);
             _.setAttribute("class", "gates-zero"), y.push(_);
-            var k = y0(c[1]);
-            k.setAttribute("class", "gates-one"), y.push(k)
+            var w = x0(c[1]);
+            w.setAttribute("class", "gates-one"), y.push(w)
         }
         var T = d + Re.controlBtnRadius,
             A = Qh(T, g),
             L = g + Re.controlBtnRadius,
             R = g + Re.classicalRegHeight / 2,
-            G = (0, be.dashedLine)(T, L, T, R, "classical-line");
+            O = (0, be.dashedLine)(T, L, T, R, "classical-line");
         d += Re.controlBtnOffset;
         var P = (0, be.dashedLine)(T, R, d, R, "classical-line");
-        m = m - Re.controlBtnOffset + (e - Re.groupBoxPadding) * 2, d += Re.groupBoxPadding - e;
+        f = f - Re.controlBtnOffset + (e - Re.groupBoxPadding) * 2, d += Re.groupBoxPadding - e;
         var I = l[0] - Re.gateHeight / 2 - e,
             Y = l[1] - l[0] + Re.gateHeight + e * 2,
-            re = (0, be.dashedBox)(d, I, m, Y, "classical-container");
-        y.push.apply(y, [P, G, A, re]);
+            re = (0, be.dashedBox)(d, I, f, Y, "classical-container");
+        y.push.apply(y, [P, O, A, re]);
         var te = {
             class: "classically-controlled-group classically-controlled-unknown"
         };
         return a != null && Object.entries(a).forEach(function(j) {
             var ne = j[0],
                 pe = j[1];
             return te["data-".concat(ne)] = pe
         }), (0, be.group)(y, te)
     };
-    Le._classicalControlled = Wa;
+    Le._classicalControlled = Xa;
     var Qh = function(r, e, i) {
         return i === void 0 && (i = Re.controlBtnRadius), (0, be.group)([(0, be.circle)(r, e, i), (0, be.text)("?", r, e, Re.labelFontSize)], {
             class: "classically-controlled-btn"
         })
     }
 });
-var Ja = W(Wt => {
+var rs = W(Yt => {
     "use strict";
-    Object.defineProperty(Wt, "__esModule", {
+    Object.defineProperty(Yt, "__esModule", {
         value: !0
     });
-    Wt._qubitRegister = Wt._classicalRegister = Wt.formatRegisters = void 0;
-    var Qa = Ut(),
-        Zh = hr(),
-        Lt = b0(),
-        Xh = function(r, e, i) {
+    Yt._qubitRegister = Yt._classicalRegister = Yt.formatRegisters = void 0;
+    var Ka = Wt(),
+        Xh = hr(),
+        Lt = y0(),
+        Jh = function(r, e, i) {
             var a = [];
-            for (var l in r) a.push(Xa(Number(l), i, r[l].y));
+            for (var l in r) a.push(ts(Number(l), i, r[l].y));
             return e.forEach(function(c) {
                 var d = c.type,
-                    m = c.x,
+                    f = c.x,
                     g = c.targetsY,
                     y = c.controlsY;
-                if (d === Zh.GateType.Measure) {
+                if (d === Xh.GateType.Measure) {
                     var _ = y[0];
-                    g.forEach(function(k) {
-                        a.push(Za(m, _, i, k))
+                    g.forEach(function(w) {
+                        a.push(es(f, _, i, w))
                     })
                 }
             }), (0, Lt.group)(a)
         };
-    Wt.formatRegisters = Xh;
-    var Za = function(r, e, i, a) {
+    Yt.formatRegisters = Jh;
+    var es = function(r, e, i, a) {
         var l = 1,
             c = (0, Lt.line)(r + l, e, r + l, a - l, "register-classical"),
             d = (0, Lt.line)(r - l, e, r - l, a + l, "register-classical"),
-            m = (0, Lt.line)(r + l, a - l, i, a - l, "register-classical"),
+            f = (0, Lt.line)(r + l, a - l, i, a - l, "register-classical"),
             g = (0, Lt.line)(r - l, a + l, i, a + l, "register-classical");
-        return (0, Lt.group)([c, d, m, g])
+        return (0, Lt.group)([c, d, f, g])
     };
-    Wt._classicalRegister = Za;
-    var Xa = function(r, e, i, a) {
+    Yt._classicalRegister = es;
+    var ts = function(r, e, i, a) {
         a === void 0 && (a = 16);
-        var l = (0, Lt.line)(Qa.regLineStart, i, e, i),
-            c = (0, Lt.text)("q".concat(r), Qa.regLineStart, i - a);
+        var l = (0, Lt.line)(Ka.regLineStart, i, e, i),
+            c = (0, Lt.text)("q".concat(r), Ka.regLineStart, i - a);
         return c.setAttribute("dominant-baseline", "hanging"), c.setAttribute("text-anchor", "start"), c.setAttribute("font-size", "75%"), (0, Lt.group)([l, c])
     };
-    Wt._qubitRegister = Xa
+    Yt._qubitRegister = ts
 });
-var Vn = W(Fr => {
+var Un = W(Fr => {
     "use strict";
     Object.defineProperty(Fr, "__esModule", {
         value: !0
     });
     Fr.ConditionalRender = void 0;
-    var Jh;
+    var Kh;
     (function(r) {
         r[r.Always = 0] = "Always", r[r.OnZero = 1] = "OnZero", r[r.OnOne = 2] = "OnOne", r[r.AsGroup = 3] = "AsGroup"
-    })(Jh = Fr.ConditionalRender || (Fr.ConditionalRender = {}))
+    })(Kh = Fr.ConditionalRender || (Fr.ConditionalRender = {}))
 });
-var Wn = W(Yt => {
+var Zn = W(Zt => {
     "use strict";
-    Object.defineProperty(Yt, "__esModule", {
+    Object.defineProperty(Zt, "__esModule", {
         value: !0
     });
-    Yt._getStringWidth = Yt.getGateWidth = Yt.createUUID = void 0;
-    var jn = hr(),
-        Br = Ut(),
-        Kh = function() {
+    Zt._getStringWidth = Zt.getGateWidth = Zt.createUUID = void 0;
+    var Wn = hr(),
+        Br = Wt(),
+        ed = function() {
             return "xxxxxxxx-xxxx-4xxx-yxxx-xxxxxxxxxxxx".replace(/[xy]/g, function(r) {
                 var e = Math.random() * 16 | 0,
                     i = r == "x" ? e : e & 3 | 8;
                 return i.toString(16)
             })
         };
-    Yt.createUUID = Kh;
-    var ed = function(r) {
+    Zt.createUUID = ed;
+    var td = function(r) {
         var e = r.type,
             i = r.label,
             a = r.displayArgs,
             l = r.width;
         if (l > 0) return l;
         switch (e) {
-            case jn.GateType.Measure:
-            case jn.GateType.Cnot:
-            case jn.GateType.Swap:
+            case Wn.GateType.Measure:
+            case Wn.GateType.Cnot:
+            case Wn.GateType.Swap:
                 return Br.minGateWidth;
             default:
-                var c = Un(i),
-                    d = a != null ? Un(a, Br.argsFontSize) : 0,
-                    m = Math.max(c, d) + Br.labelPadding * 2;
-                return Math.max(Br.minGateWidth, m)
+                var c = Yn(i),
+                    d = a != null ? Yn(a, Br.argsFontSize) : 0,
+                    f = Math.max(c, d) + Br.labelPadding * 2;
+                return Math.max(Br.minGateWidth, f)
         }
     };
-    Yt.getGateWidth = ed;
-    var Un = function(r, e) {
+    Zt.getGateWidth = td;
+    var Yn = function(r, e) {
         e === void 0 && (e = Br.labelFontSize);
         var i = document.createElement("canvas"),
             a = i.getContext("2d");
         if (a == null) throw new Error("Null canvas");
         a.font = "".concat(e, "px Arial");
         var l = a.measureText(r);
         return l.width
     };
-    Yt._getStringWidth = Un
+    Zt._getStringWidth = Yn
 });
-var os = W(Pe => {
+var cs = W(Pe => {
     "use strict";
-    var v0 = Pe && Pe.__assign || function() {
-            return v0 = Object.assign || function(r) {
+    var w0 = Pe && Pe.__assign || function() {
+            return w0 = Object.assign || function(r) {
                 for (var e, i = 1, a = arguments.length; i < a; i++) {
                     e = arguments[i];
                     for (var l in e) Object.prototype.hasOwnProperty.call(e, l) && (r[l] = e[l])
                 }
                 return r
-            }, v0.apply(this, arguments)
+            }, w0.apply(this, arguments)
         },
         dr = Pe && Pe.__spreadArray || function(r, e, i) {
             if (i || arguments.length === 2)
                 for (var a = 0, l = e.length, c; a < l; a++)(c || !(a in e)) && (c || (c = Array.prototype.slice.call(e, 0, a)), c[a] = e[a]);
             return r.concat(c || Array.prototype.slice.call(e))
         };
     Object.defineProperty(Pe, "__esModule", {
         value: !0
     });
     Pe._offsetChildrenX = Pe._fillMetadataX = Pe._splitTargetsY = Pe._getRegY = Pe._opToMetadata = Pe._getClassicalRegStart = Pe._alignOps = Pe._groupOperations = Pe.processOperations = void 0;
-    var ot = Ut(),
-        Yn = Vn(),
+    var ot = Wt(),
+        Qn = Un(),
         rt = hr(),
-        nr = On(),
-        td = Wn(),
-        x0 = function(r, e) {
+        ir = $n(),
+        rd = Zn(),
+        v0 = function(r, e) {
             if (r.length === 0) return {
                 metadataList: [],
                 svgWidth: ot.startX
             };
-            var i = Ka(r, e),
-                a = es(i),
-                l = Math.max.apply(Math, dr([0], a.map(function(k) {
-                    return k.length
+            var i = ns(r, e),
+                a = is(i),
+                l = Math.max.apply(Math, dr([0], a.map(function(w) {
+                    return w.length
                 }), !1)),
                 c = new Array(l).fill(ot.minGateWidth),
-                d = ts(r, a),
-                m = {},
-                g = a.map(function(k) {
-                    return k.map(function(T, A) {
+                d = os(r, a),
+                f = {},
+                g = a.map(function(w) {
+                    return w.map(function(T, A) {
                         var L = null;
-                        T != null && !m.hasOwnProperty(T) && (L = r[T], m[T] = !0);
-                        var R = rs(L, e);
+                        T != null && !f.hasOwnProperty(T) && (L = r[T], f[T] = !0);
+                        var R = as(L, e);
                         if (L != null && [rt.GateType.Unitary, rt.GateType.ControlledUnitary].includes(R.type)) {
-                            var G = d.filter(function(P) {
+                            var O = d.filter(function(P) {
                                 var I = P[0],
                                     Y = P[1];
                                 return I <= A
                             }).map(function(P) {
                                 var I = P[0],
                                     Y = P[1];
                                 if (Y.cId == null) throw new Error("Could not find cId for classical register.");
                                 var re = e[Y.qId].children;
                                 if (re == null) throw new Error("Failed to find classical registers for qubit ID ".concat(Y.qId, "."));
                                 return re[Y.cId].y
                             });
-                            R.targetsY = ns(L.targets, G, e)
+                            R.targetsY = ss(L.targets, O, e)
                         }
                         return R.width > c[A] && (c[A] = R.width), R
                     })
                 }),
-                y = is(g, c),
-                _ = g.flat().filter(function(k) {
-                    var T = k.type;
+                y = ls(g, c),
+                _ = g.flat().filter(function(w) {
+                    var T = w.type;
                     return T != rt.GateType.Invalid
                 });
             return {
                 metadataList: _,
                 svgWidth: y
             }
         };
-    Pe.processOperations = x0;
-    var Ka = function(r, e) {
+    Pe.processOperations = v0;
+    var ns = function(r, e) {
         var i = Math.max.apply(Math, dr([-1], Object.keys(e).map(Number), !1)) + 1,
             a = Array.from(Array(i), function() {
                 return new Array(0)
             });
         return r.forEach(function(l, c) {
             var d = l.targets,
-                m = l.controls,
-                g = m || [],
-                y = dr(dr([], g, !0), d, !0).filter(function(G) {
-                    var P = G.type;
-                    return (P || nr.RegisterType.Qubit) === nr.RegisterType.Qubit
+                f = l.controls,
+                g = f || [],
+                y = dr(dr([], g, !0), d, !0).filter(function(O) {
+                    var P = O.type;
+                    return (P || ir.RegisterType.Qubit) === ir.RegisterType.Qubit
                 }),
-                _ = y.map(function(G) {
-                    var P = G.qId;
+                _ = y.map(function(O) {
+                    var P = O.qId;
                     return P
                 }),
-                k = g.filter(function(G) {
-                    var P = G.type;
-                    return (P || nr.RegisterType.Qubit) === nr.RegisterType.Classical
+                w = g.filter(function(O) {
+                    var P = O.type;
+                    return (P || ir.RegisterType.Qubit) === ir.RegisterType.Classical
                 }),
-                T = k.length > 0;
+                T = w.length > 0;
             if (!(!T && y.length === 0))
                 for (var A = T ? 0 : Math.min.apply(Math, _), L = T ? i - 1 : Math.max.apply(Math, _), R = A; R <= L; R++) a[R].push(c)
         }), a
     };
-    Pe._groupOperations = Ka;
-    var es = function(r) {
+    Pe._groupOperations = ns;
+    var is = function(r) {
         for (var e = Math.max.apply(Math, dr([0], r.map(function(d) {
                 return d.length
             }), !1)), i = 0, a = JSON.parse(JSON.stringify(r)); i < e;) {
             for (var l = function(d) {
-                    var m = a[d];
-                    if (m.length <= i) return "continue";
-                    var g = m[i],
-                        y = a.map(function(k) {
-                            return k.indexOf(g)
+                    var f = a[d];
+                    if (f.length <= i) return "continue";
+                    var g = f[i],
+                        y = a.map(function(w) {
+                            return w.indexOf(g)
                         }),
                         _ = Math.max.apply(Math, dr([-1], y, !1));
                     i < _ && (a[d].splice(i, 0, null), e = Math.max(e, a[d].length))
                 }, c = 0; c < a.length; c++) l(c);
             i++
         }
         return a
     };
-    Pe._alignOps = es;
-    var ts = function(r, e) {
+    Pe._alignOps = is;
+    var os = function(r, e) {
         var i = [];
         return e.forEach(function(a) {
             for (var l = function(d) {
-                    var m = a[d];
-                    if (m != null && r[m].isMeasurement) {
-                        var g = r[m].targets.filter(function(y) {
-                            return y.type === nr.RegisterType.Classical
+                    var f = a[d];
+                    if (f != null && r[f].isMeasurement) {
+                        var g = r[f].targets.filter(function(y) {
+                            return y.type === ir.RegisterType.Classical
                         });
                         g.forEach(function(y) {
                             return i.push([d, y])
                         })
                     }
                 }, c = 0; c < a.length; c++) l(c)
         }), i
     };
-    Pe._getClassicalRegStart = ts;
-    var rs = function(r, e) {
+    Pe._getClassicalRegStart = os;
+    var as = function(r, e) {
         var i = {
             type: rt.GateType.Invalid,
             x: 0,
             controlsY: [],
             targetsY: [],
             label: "",
             width: -1
         };
         if (r == null) return i;
         var a = r.gate,
             l = r.dataAttributes,
             c = r.displayArgs,
             d = r.isMeasurement,
-            m = r.isConditional,
+            f = r.isConditional,
             g = r.isControlled,
             y = r.isAdjoint,
             _ = r.controls,
-            k = r.targets,
+            w = r.targets,
             T = r.children,
             A = r.conditionalRender;
         if (i.controlsY = _?.map(function(ne) {
-                return w0(ne, e)
-            }) || [], i.targetsY = k.map(function(ne) {
-                return w0(ne, e)
-            }), m) {
+                return k0(ne, e)
+            }) || [], i.targetsY = w.map(function(ne) {
+                return k0(ne, e)
+            }), f) {
             if (T == null || T.length == 0) throw new Error("No children operations found for classically-controlled operation.");
             var L = T.filter(function(ne) {
-                    return ne.conditionalRender !== Yn.ConditionalRender.OnOne
+                    return ne.conditionalRender !== Qn.ConditionalRender.OnOne
                 }),
-                R = x0(L, e),
-                G = R.metadataList,
+                R = v0(L, e),
+                O = R.metadataList,
                 P = R.svgWidth,
                 I = T.filter(function(ne) {
-                    return ne.conditionalRender !== Yn.ConditionalRender.OnZero
+                    return ne.conditionalRender !== Qn.ConditionalRender.OnZero
                 });
-            R = x0(I, e);
+            R = v0(I, e);
             var Y = R.metadataList,
                 re = R.svgWidth,
                 te = Math.max(P, re) - ot.startX - ot.gatePadding * 2;
-            i.type = rt.GateType.ClassicalControlled, i.children = [G, Y], i.width = te + ot.controlBtnOffset + ot.groupBoxPadding * 2;
+            i.type = rt.GateType.ClassicalControlled, i.children = [O, Y], i.width = te + ot.controlBtnOffset + ot.groupBoxPadding * 2;
             var j = Object.values(e).map(function(ne) {
                 var pe = ne.y;
                 return pe
             });
             j.length > 0 && (i.targetsY = [Math.min.apply(Math, j), Math.max.apply(Math, j)])
-        } else if (A == Yn.ConditionalRender.AsGroup && (T?.length || 0) > 0) {
-            var R = x0(T, e);
+        } else if (A == Qn.ConditionalRender.AsGroup && (T?.length || 0) > 0) {
+            var R = v0(T, e);
             i.type = rt.GateType.Group, i.children = R.metadataList, i.dataAttributes = {
                 expanded: "true"
             }, i.width = R.svgWidth - ot.startX + (ot.groupBoxPadding - ot.gatePadding) * 2
         } else d ? i.type = rt.GateType.Measure : a === "SWAP" ? i.type = rt.GateType.Swap : g ? (i.type = a === "X" ? rt.GateType.Cnot : rt.GateType.ControlledUnitary, i.label = a) : a === "X" ? (i.type = rt.GateType.X, i.label = a) : (i.type = rt.GateType.Unitary, i.label = a);
-        return y && i.label.length > 0 && (i.label += "'"), c != null && (i.displayArgs = c), i.width = (0, td.getGateWidth)(i), l != null && (i.dataAttributes = v0(v0({}, i.dataAttributes), l)), i
+        return y && i.label.length > 0 && (i.label += "'"), c != null && (i.displayArgs = c), i.width = (0, rd.getGateWidth)(i), l != null && (i.dataAttributes = w0(w0({}, i.dataAttributes), l)), i
     };
-    Pe._opToMetadata = rs;
-    var w0 = function(r, e) {
+    Pe._opToMetadata = as;
+    var k0 = function(r, e) {
         var i = r.type,
             a = r.qId,
             l = r.cId;
         if (!e.hasOwnProperty(a)) throw new Error("ERROR: Qubit register with ID ".concat(a, " not found."));
         var c = e[a],
             d = c.y,
-            m = c.children;
+            f = c.children;
         switch (i) {
             case void 0:
-            case nr.RegisterType.Qubit:
+            case ir.RegisterType.Qubit:
                 return d;
-            case nr.RegisterType.Classical:
-                if (m == null) throw new Error("ERROR: No classical registers found for qubit ID ".concat(a, "."));
+            case ir.RegisterType.Classical:
+                if (f == null) throw new Error("ERROR: No classical registers found for qubit ID ".concat(a, "."));
                 if (l == null) throw new Error("ERROR: No ID defined for classical register associated with qubit ID ".concat(a, "."));
-                if (m.length <= l) throw new Error("ERROR: Classical register ID ".concat(l, " invalid for qubit ID ").concat(a, " with ").concat(m.length, " classical register(s)."));
-                return m[l].y;
+                if (f.length <= l) throw new Error("ERROR: Classical register ID ".concat(l, " invalid for qubit ID ").concat(a, " with ").concat(f.length, " classical register(s)."));
+                return f[l].y;
             default:
                 throw new Error("ERROR: Unknown register type ".concat(i, "."))
         }
     };
-    Pe._getRegY = w0;
-    var ns = function(r, e, i) {
+    Pe._getRegY = k0;
+    var ss = function(r, e, i) {
         if (r.length === 0) return [];
         var a = Object.keys(i).map(Number);
-        a.sort(function(m, g) {
-            return i[m].y - i[g].y
+        a.sort(function(f, g) {
+            return i[f].y - i[g].y
         });
         var l = {};
-        a.forEach(function(m, g) {
-            return l[m] = g
-        }), r = r.slice(), r.sort(function(m, g) {
-            var y = l[m.qId] - l[g.qId];
-            return y === 0 && m.cId != null && g.cId != null ? m.cId - g.cId : y
-        }), e = e.slice(), e.sort(function(m, g) {
-            return m - g
+        a.forEach(function(f, g) {
+            return l[f] = g
+        }), r = r.slice(), r.sort(function(f, g) {
+            var y = l[f.qId] - l[g.qId];
+            return y === 0 && f.cId != null && g.cId != null ? f.cId - g.cId : y
+        }), e = e.slice(), e.sort(function(f, g) {
+            return f - g
         });
         var c = 0,
             d = 0;
-        return r.reduce(function(m, g) {
-            var y = w0(g, i),
+        return r.reduce(function(f, g) {
+            var y = k0(g, i),
                 _ = l[g.qId];
-            for (m.length === 0 || _ > c + 1 || e[0] > d && e[0] < y ? m.push([y]) : m[m.length - 1].push(y), c = _, d = y; e.length > 0 && e[0] <= y;) e.shift();
-            return m
+            for (f.length === 0 || _ > c + 1 || e[0] > d && e[0] < y ? f.push([y]) : f[f.length - 1].push(y), c = _, d = y; e.length > 0 && e[0] <= y;) e.shift();
+            return f
         }, [])
     };
-    Pe._splitTargetsY = ns;
-    var is = function(r, e) {
+    Pe._splitTargetsY = ss;
+    var ls = function(r, e) {
         var i = ot.startX,
             a = e.map(function(c) {
                 var d = i;
                 return i += c + ot.gatePadding * 2, d
             }),
             l = i;
         return r.forEach(function(c) {
-            return c.forEach(function(d, m) {
-                var g = a[m];
+            return c.forEach(function(d, f) {
+                var g = a[f];
                 switch (d.type) {
                     case rt.GateType.ClassicalControlled:
                     case rt.GateType.Group:
                         var y = g - ot.startX + ot.groupBoxPadding;
-                        d.type === rt.GateType.ClassicalControlled && (y += ot.controlBtnOffset), Qn(d.children, y), d.x = g;
+                        d.type === rt.GateType.ClassicalControlled && (y += ot.controlBtnOffset), Xn(d.children, y), d.x = g;
                         break;
                     default:
-                        d.x = g + e[m] / 2;
+                        d.x = g + e[f] / 2;
                         break
                 }
             })
         }), l
     };
-    Pe._fillMetadataX = is;
-    var Qn = function(r, e) {
+    Pe._fillMetadataX = ls;
+    var Xn = function(r, e) {
         r?.flat().forEach(function(i) {
-            i.x += e, Qn(i.children, e)
+            i.x += e, Xn(i.children, e)
         })
     };
-    Pe._offsetChildrenX = Qn
+    Pe._offsetChildrenX = Xn
 });
-var Zn = W(Qt => {
+var Jn = W(Qt => {
     "use strict";
-    var k0 = Qt && Qt.__assign || function() {
-        return k0 = Object.assign || function(r) {
+    var _0 = Qt && Qt.__assign || function() {
+        return _0 = Object.assign || function(r) {
             for (var e, i = 1, a = arguments.length; i < a; i++) {
                 e = arguments[i];
                 for (var l in e) Object.prototype.hasOwnProperty.call(e, l) && (r[l] = e[l])
             }
             return r
-        }, k0.apply(this, arguments)
+        }, _0.apply(this, arguments)
     };
     Object.defineProperty(Qt, "__esModule", {
         value: !0
     });
     Qt.style = Qt.STYLES = void 0;
-    var as = {
+    var us = {
             lineStroke: "#000000",
             lineWidth: 1,
             textColour: "#000000",
             unitary: "#D9F1FA",
             oplus: "#FFFFFF",
             measure: "#FFDE86",
             classicalUnknown: "#E5E5E5",
             classicalZero: "#C40000",
             classicalOne: "#4059BD",
             classicalZeroText: "#FFFFFF",
             classicalOneText: "#FFFFFF"
         },
-        rd = {
+        nd = {
             lineStroke: "#000000",
             lineWidth: 1,
             textColour: "#000000",
             unitary: "#FFFFFF",
             oplus: "#FFFFFF",
             measure: "#FFFFFF",
             classicalUnknown: "#FFFFFF",
             classicalZero: "#000000",
             classicalOne: "#000000",
             classicalZeroText: "#FFFFFF",
             classicalOneText: "#FFFFFF"
         },
-        nd = {
+        id = {
             lineStroke: "#FFFFFF",
             lineWidth: 1,
             textColour: "#FFFFFF",
             unitary: "#000000",
             oplus: "#000000",
             measure: "#000000",
             classicalUnknown: "#000000",
             classicalZero: "#FFFFFF",
             classicalOne: "#FFFFFF",
             classicalZeroText: "#000000",
             classicalOneText: "#000000"
         };
     Qt.STYLES = {
-        Default: as,
-        BlackAndWhite: rd,
-        Inverted: nd
+        Default: us,
+        BlackAndWhite: nd,
+        Inverted: id
     };
-    var id = function(r) {
+    var od = function(r) {
         r === void 0 && (r = {});
-        var e = k0(k0({}, as), r);
-        return "".concat(od(e), `
-    `).concat(ad(e), `
-    `).concat(sd)
+        var e = _0(_0({}, us), r);
+        return "".concat(ad(e), `
+    `).concat(sd(e), `
+    `).concat(ld)
     };
-    Qt.style = id;
-    var od = function(r) {
+    Qt.style = od;
+    var ad = function(r) {
             return `
     line,
     circle,
     rect {
         stroke: `.concat(r.lineStroke, `;
         stroke-width: `).concat(r.lineWidth, `;
     }
@@ -960,15 +960,15 @@
         fill: none;
         stroke-width: `).concat(r.lineWidth, `;
     }
     .register-classical {
         stroke-width: `).concat((r.lineWidth || 0) / 2, `;
     }`)
         },
-        ad = function(r) {
+        sd = function(r) {
             var e = `
     .classically-controlled-one .classical-container,
     .classically-controlled-one .classical-line {
         stroke: `.concat(r.classicalOne, `;
         stroke-width: `).concat((r.lineWidth || 0) + .3, `;
         fill: `).concat(r.classicalOne, `;
         fill-opacity: 0.1;
@@ -1017,15 +1017,15 @@
         opacity: 0.25;
     }
 
     `.concat(e, `
     `).concat(i, `
     `).concat(a)
         },
-        sd = `
+        ld = `
     .qviz .gate-collapse,
     .qviz .gate-expand {
         opacity: 0;
         transition: opacity 1s;
     }
 
     .qviz:hover .gate-collapse,
@@ -1055,49 +1055,49 @@
     .gate:hover > .gate-collapse,
     .gate:hover > .gate-expand {
         visibility: visible;
         opacity: 1;
         transition: opacity 1s;
     }`
 });
-var ss = W(S0 => {
+var hs = W(C0 => {
     "use strict";
-    Object.defineProperty(S0, "__esModule", {
+    Object.defineProperty(C0, "__esModule", {
         value: !0
     });
-    S0.Sqore = void 0;
-    var ld = Ia(),
-        cd = Ya(),
+    C0.Sqore = void 0;
+    var cd = Ga(),
         ud = Ja(),
-        hd = os(),
-        _0 = Vn(),
-        dd = hr(),
-        Xn = Zn(),
-        md = Wn(),
-        pd = Ut(),
-        fd = function() {
+        hd = rs(),
+        dd = cs(),
+        S0 = Un(),
+        md = hr(),
+        Kn = Jn(),
+        pd = Zn(),
+        fd = Wt(),
+        gd = function() {
             function r(e, i) {
                 i === void 0 && (i = {}), this.style = {}, this.gateRegistry = {}, this.circuit = e, this.style = this.getStyle(i)
             }
             return r.prototype.draw = function(e, i) {
                 var a = this;
                 if (i === void 0 && (i = 0), e == null) throw new Error("Container not provided.");
                 var l = JSON.parse(JSON.stringify(this.circuit));
-                if (l.operations.forEach(function(d, m) {
-                        return a.fillGateRegistry(d, m.toString())
+                if (l.operations.forEach(function(d, f) {
+                        return a.fillGateRegistry(d, f.toString())
                     }), l.operations = this.selectOpsAtDepth(l.operations, i), l.operations.length == 1 && l.operations[0].dataAttributes != null && l.operations[0].dataAttributes.hasOwnProperty("id")) {
                     var c = l.operations[0].dataAttributes.id;
                     this.expandOperation(l.operations, c)
                 }
                 this.renderCircuit(e, l)
             }, r.prototype.getStyle = function(e) {
                 if (e === void 0 && (e = {}), typeof e == "string" || e instanceof String) {
                     var i = e;
-                    if (!Xn.STYLES.hasOwnProperty(i)) return console.error("No style ".concat(i, " found in STYLES.")), {};
-                    e = Xn.STYLES[i]
+                    if (!Kn.STYLES.hasOwnProperty(i)) return console.error("No style ".concat(i, " found in STYLES.")), {};
+                    e = Kn.STYLES[i]
                 }
                 return e
             }, r.prototype.renderCircuit = function(e, i) {
                 var a = this.compose(i),
                     l = this.generateSvg(a);
                 e.innerHTML = "", e.appendChild(l), this.addGateClickHandlers(e, i)
             }, r.prototype.compose = function(e) {
@@ -1111,42 +1111,42 @@
                     },
                     a = function(P) {
                         var I = [];
                         return i(I, P), I
                     },
                     l = e.qubits,
                     c = e.operations,
-                    d = (0, ld.formatInputs)(l),
-                    m = d.qubitWires,
+                    d = (0, cd.formatInputs)(l),
+                    f = d.qubitWires,
                     g = d.registers,
                     y = d.svgHeight,
-                    _ = (0, hd.processOperations)(c, g),
-                    k = _.metadataList,
+                    _ = (0, dd.processOperations)(c, g),
+                    w = _.metadataList,
                     T = _.svgWidth,
-                    A = (0, cd.formatGates)(k),
-                    L = a(k).filter(function(P) {
+                    A = (0, ud.formatGates)(w),
+                    L = a(w).filter(function(P) {
                         var I = P.type;
-                        return I === dd.GateType.Measure
+                        return I === md.GateType.Measure
                     }),
-                    R = (0, ud.formatRegisters)(g, L, T),
-                    G = {
+                    R = (0, hd.formatRegisters)(g, L, T),
+                    O = {
                         width: T,
                         height: y,
-                        elements: [m, R, A]
+                        elements: [f, R, A]
                     };
-                return G
+                return O
             }, r.prototype.generateSvg = function(e) {
                 var i = e.width,
                     a = e.height,
                     l = e.elements,
-                    c = (0, md.createUUID)(),
-                    d = document.createElementNS(pd.svgNS, "svg");
+                    c = (0, pd.createUUID)(),
+                    d = document.createElementNS(fd.svgNS, "svg");
                 d.setAttribute("id", c), d.setAttribute("class", "qviz"), d.setAttribute("width", i.toString()), d.setAttribute("height", a.toString()), d.style.setProperty("max-width", "fit-content");
-                var m = document.createElement("style");
-                return m.innerHTML = (0, Xn.style)(this.style), d.appendChild(m), l.forEach(function(g) {
+                var f = document.createElement("style");
+                return f.innerHTML = (0, Kn.style)(this.style), d.appendChild(f), l.forEach(function(g) {
                     return d.appendChild(g)
                 }), d
             }, r.prototype.fillGateRegistry = function(e, i) {
                 var a = this,
                     l;
                 e.dataAttributes == null && (e.dataAttributes = {}), e.dataAttributes.id = i, e.dataAttributes["zoom-out"] = "false", this.gateRegistry[i] = e, (l = e.children) === null || l === void 0 || l.forEach(function(c, d) {
                     a.fillGateRegistry(c, "".concat(i, "-").concat(d)), c.dataAttributes == null && (c.dataAttributes = {}), c.dataAttributes["zoom-out"] = "true"
@@ -1161,18 +1161,18 @@
                 this.addClassicalControlHandlers(e), this.addZoomHandlers(e, i)
             }, r.prototype.addClassicalControlHandlers = function(e) {
                 e.querySelectorAll(".classically-controlled-btn").forEach(function(i) {
                     i.addEventListener("click", function(a) {
                         var l, c = i.querySelector("text"),
                             d = i.parentElement;
                         if (!(c == null || d == null)) {
-                            var m = (l = c.firstChild) === null || l === void 0 ? void 0 : l.nodeValue,
+                            var f = (l = c.firstChild) === null || l === void 0 ? void 0 : l.nodeValue,
                                 g = d?.querySelector(".gates-zero"),
                                 y = d?.querySelector(".gates-one");
-                            switch (m) {
+                            switch (f) {
                                 case "?":
                                     c.childNodes[0].nodeValue = "1", d.classList.remove("classically-controlled-unknown"), d.classList.remove("classically-controlled-zero"), d.classList.add("classically-controlled-one"), g?.classList.add("hidden"), y?.classList.remove("hidden");
                                     break;
                                 case "1":
                                     c.childNodes[0].nodeValue = "0", d.classList.remove("classically-controlled-unknown"), d.classList.add("classically-controlled-zero"), d.classList.remove("classically-controlled-one"), g?.classList.remove("hidden"), y?.classList.add("hidden");
                                     break;
                                 case "0":
@@ -1183,59 +1183,59 @@
                         }
                     })
                 })
             }, r.prototype.addZoomHandlers = function(e, i) {
                 var a = this;
                 e.querySelectorAll(".gate .gate-control").forEach(function(l) {
                     l.addEventListener("click", function(c) {
-                        var d, m = (d = l.parentElement) === null || d === void 0 ? void 0 : d.getAttribute("data-id");
-                        typeof m == "string" && (l.classList.contains("gate-collapse") ? a.collapseOperation(i.operations, m) : l.classList.contains("gate-expand") && a.expandOperation(i.operations, m), a.renderCircuit(e, i), c.stopPropagation())
+                        var d, f = (d = l.parentElement) === null || d === void 0 ? void 0 : d.getAttribute("data-id");
+                        typeof f == "string" && (l.classList.contains("gate-collapse") ? a.collapseOperation(i.operations, f) : l.classList.contains("gate-expand") && a.expandOperation(i.operations, f), a.renderCircuit(e, i), c.stopPropagation())
                     })
                 })
             }, r.prototype.expandOperation = function(e, i) {
                 var a = this;
                 e.forEach(function(l) {
-                    if (l.conditionalRender === _0.ConditionalRender.AsGroup && a.expandOperation(l.children || [], i), l.dataAttributes == null) return l;
+                    if (l.conditionalRender === S0.ConditionalRender.AsGroup && a.expandOperation(l.children || [], i), l.dataAttributes == null) return l;
                     var c = l.dataAttributes.id;
-                    c === i && l.children != null && (l.conditionalRender = _0.ConditionalRender.AsGroup, l.dataAttributes.expanded = "true")
+                    c === i && l.children != null && (l.conditionalRender = S0.ConditionalRender.AsGroup, l.dataAttributes.expanded = "true")
                 })
             }, r.prototype.collapseOperation = function(e, i) {
                 var a = this;
                 e.forEach(function(l) {
-                    if (l.conditionalRender === _0.ConditionalRender.AsGroup && a.collapseOperation(l.children || [], i), l.dataAttributes == null) return l;
+                    if (l.conditionalRender === S0.ConditionalRender.AsGroup && a.collapseOperation(l.children || [], i), l.dataAttributes == null) return l;
                     var c = l.dataAttributes.id;
-                    c.startsWith(i) && (l.conditionalRender = _0.ConditionalRender.Always, delete l.dataAttributes.expanded)
+                    c.startsWith(i) && (l.conditionalRender = S0.ConditionalRender.Always, delete l.dataAttributes.expanded)
                 })
             }, r
         }();
-    S0.Sqore = fd
+    C0.Sqore = gd
 });
-var ls = W(mr => {
+var ds = W(mr => {
     "use strict";
     Object.defineProperty(mr, "__esModule", {
         value: !0
     });
     mr.STYLES = mr.draw = void 0;
-    var gd = ss(),
-        bd = function(r, e, i, a) {
+    var bd = hs(),
+        yd = function(r, e, i, a) {
             i === void 0 && (i = {}), a === void 0 && (a = 0);
-            var l = new gd.Sqore(r, i);
+            var l = new bd.Sqore(r, i);
             l.draw(e, a)
         };
-    mr.draw = bd;
-    var yd = Zn();
+    mr.draw = yd;
+    var xd = Jn();
     Object.defineProperty(mr, "STYLES", {
         enumerable: !0,
         get: function() {
-            return yd.STYLES
+            return xd.STYLES
         }
     })
 });
-var ds = W((q4, xd) => {
-    xd.exports = {
+var ps = W((P4, _d) => {
+    _d.exports = {
         Aacute: "\xC1",
         aacute: "\xE1",
         Abreve: "\u0102",
         abreve: "\u0103",
         ac: "\u223E",
         acd: "\u223F",
         acE: "\u223E\u0333",
@@ -3356,318 +3356,318 @@
         Zopf: "\u2124",
         Zscr: "\u{1D4B5}",
         zscr: "\u{1D4CF}",
         zwj: "\u200D",
         zwnj: "\u200C"
     }
 });
-var Kn = W((M4, ms) => {
+var ni = W((I4, fs) => {
     "use strict";
-    ms.exports = ds()
+    fs.exports = ps()
 });
-var C0 = W((E4, ps) => {
-    ps.exports = /[!-#%-\*,-\/:;\?@\[-\]_\{\}\xA1\xA7\xAB\xB6\xB7\xBB\xBF\u037E\u0387\u055A-\u055F\u0589\u058A\u05BE\u05C0\u05C3\u05C6\u05F3\u05F4\u0609\u060A\u060C\u060D\u061B\u061E\u061F\u066A-\u066D\u06D4\u0700-\u070D\u07F7-\u07F9\u0830-\u083E\u085E\u0964\u0965\u0970\u09FD\u0A76\u0AF0\u0C84\u0DF4\u0E4F\u0E5A\u0E5B\u0F04-\u0F12\u0F14\u0F3A-\u0F3D\u0F85\u0FD0-\u0FD4\u0FD9\u0FDA\u104A-\u104F\u10FB\u1360-\u1368\u1400\u166D\u166E\u169B\u169C\u16EB-\u16ED\u1735\u1736\u17D4-\u17D6\u17D8-\u17DA\u1800-\u180A\u1944\u1945\u1A1E\u1A1F\u1AA0-\u1AA6\u1AA8-\u1AAD\u1B5A-\u1B60\u1BFC-\u1BFF\u1C3B-\u1C3F\u1C7E\u1C7F\u1CC0-\u1CC7\u1CD3\u2010-\u2027\u2030-\u2043\u2045-\u2051\u2053-\u205E\u207D\u207E\u208D\u208E\u2308-\u230B\u2329\u232A\u2768-\u2775\u27C5\u27C6\u27E6-\u27EF\u2983-\u2998\u29D8-\u29DB\u29FC\u29FD\u2CF9-\u2CFC\u2CFE\u2CFF\u2D70\u2E00-\u2E2E\u2E30-\u2E4E\u3001-\u3003\u3008-\u3011\u3014-\u301F\u3030\u303D\u30A0\u30FB\uA4FE\uA4FF\uA60D-\uA60F\uA673\uA67E\uA6F2-\uA6F7\uA874-\uA877\uA8CE\uA8CF\uA8F8-\uA8FA\uA8FC\uA92E\uA92F\uA95F\uA9C1-\uA9CD\uA9DE\uA9DF\uAA5C-\uAA5F\uAADE\uAADF\uAAF0\uAAF1\uABEB\uFD3E\uFD3F\uFE10-\uFE19\uFE30-\uFE52\uFE54-\uFE61\uFE63\uFE68\uFE6A\uFE6B\uFF01-\uFF03\uFF05-\uFF0A\uFF0C-\uFF0F\uFF1A\uFF1B\uFF1F\uFF20\uFF3B-\uFF3D\uFF3F\uFF5B\uFF5D\uFF5F-\uFF65]|\uD800[\uDD00-\uDD02\uDF9F\uDFD0]|\uD801\uDD6F|\uD802[\uDC57\uDD1F\uDD3F\uDE50-\uDE58\uDE7F\uDEF0-\uDEF6\uDF39-\uDF3F\uDF99-\uDF9C]|\uD803[\uDF55-\uDF59]|\uD804[\uDC47-\uDC4D\uDCBB\uDCBC\uDCBE-\uDCC1\uDD40-\uDD43\uDD74\uDD75\uDDC5-\uDDC8\uDDCD\uDDDB\uDDDD-\uDDDF\uDE38-\uDE3D\uDEA9]|\uD805[\uDC4B-\uDC4F\uDC5B\uDC5D\uDCC6\uDDC1-\uDDD7\uDE41-\uDE43\uDE60-\uDE6C\uDF3C-\uDF3E]|\uD806[\uDC3B\uDE3F-\uDE46\uDE9A-\uDE9C\uDE9E-\uDEA2]|\uD807[\uDC41-\uDC45\uDC70\uDC71\uDEF7\uDEF8]|\uD809[\uDC70-\uDC74]|\uD81A[\uDE6E\uDE6F\uDEF5\uDF37-\uDF3B\uDF44]|\uD81B[\uDE97-\uDE9A]|\uD82F\uDC9F|\uD836[\uDE87-\uDE8B]|\uD83A[\uDD5E\uDD5F]/
+var T0 = W((O4, gs) => {
+    gs.exports = /[!-#%-\*,-\/:;\?@\[-\]_\{\}\xA1\xA7\xAB\xB6\xB7\xBB\xBF\u037E\u0387\u055A-\u055F\u0589\u058A\u05BE\u05C0\u05C3\u05C6\u05F3\u05F4\u0609\u060A\u060C\u060D\u061B\u061E\u061F\u066A-\u066D\u06D4\u0700-\u070D\u07F7-\u07F9\u0830-\u083E\u085E\u0964\u0965\u0970\u09FD\u0A76\u0AF0\u0C84\u0DF4\u0E4F\u0E5A\u0E5B\u0F04-\u0F12\u0F14\u0F3A-\u0F3D\u0F85\u0FD0-\u0FD4\u0FD9\u0FDA\u104A-\u104F\u10FB\u1360-\u1368\u1400\u166D\u166E\u169B\u169C\u16EB-\u16ED\u1735\u1736\u17D4-\u17D6\u17D8-\u17DA\u1800-\u180A\u1944\u1945\u1A1E\u1A1F\u1AA0-\u1AA6\u1AA8-\u1AAD\u1B5A-\u1B60\u1BFC-\u1BFF\u1C3B-\u1C3F\u1C7E\u1C7F\u1CC0-\u1CC7\u1CD3\u2010-\u2027\u2030-\u2043\u2045-\u2051\u2053-\u205E\u207D\u207E\u208D\u208E\u2308-\u230B\u2329\u232A\u2768-\u2775\u27C5\u27C6\u27E6-\u27EF\u2983-\u2998\u29D8-\u29DB\u29FC\u29FD\u2CF9-\u2CFC\u2CFE\u2CFF\u2D70\u2E00-\u2E2E\u2E30-\u2E4E\u3001-\u3003\u3008-\u3011\u3014-\u301F\u3030\u303D\u30A0\u30FB\uA4FE\uA4FF\uA60D-\uA60F\uA673\uA67E\uA6F2-\uA6F7\uA874-\uA877\uA8CE\uA8CF\uA8F8-\uA8FA\uA8FC\uA92E\uA92F\uA95F\uA9C1-\uA9CD\uA9DE\uA9DF\uAA5C-\uAA5F\uAADE\uAADF\uAAF0\uAAF1\uABEB\uFD3E\uFD3F\uFE10-\uFE19\uFE30-\uFE52\uFE54-\uFE61\uFE63\uFE68\uFE6A\uFE6B\uFF01-\uFF03\uFF05-\uFF0A\uFF0C-\uFF0F\uFF1A\uFF1B\uFF1F\uFF20\uFF3B-\uFF3D\uFF3F\uFF5B\uFF5D\uFF5F-\uFF65]|\uD800[\uDD00-\uDD02\uDF9F\uDFD0]|\uD801\uDD6F|\uD802[\uDC57\uDD1F\uDD3F\uDE50-\uDE58\uDE7F\uDEF0-\uDEF6\uDF39-\uDF3F\uDF99-\uDF9C]|\uD803[\uDF55-\uDF59]|\uD804[\uDC47-\uDC4D\uDCBB\uDCBC\uDCBE-\uDCC1\uDD40-\uDD43\uDD74\uDD75\uDDC5-\uDDC8\uDDCD\uDDDB\uDDDD-\uDDDF\uDE38-\uDE3D\uDEA9]|\uD805[\uDC4B-\uDC4F\uDC5B\uDC5D\uDCC6\uDDC1-\uDDD7\uDE41-\uDE43\uDE60-\uDE6C\uDF3C-\uDF3E]|\uD806[\uDC3B\uDE3F-\uDE46\uDE9A-\uDE9C\uDE9E-\uDEA2]|\uD807[\uDC41-\uDC45\uDC70\uDC71\uDEF7\uDEF8]|\uD809[\uDC70-\uDC74]|\uD81A[\uDE6E\uDE6F\uDEF5\uDF37-\uDF3B\uDF44]|\uD81B[\uDE97-\uDE9A]|\uD82F\uDC9F|\uD836[\uDE87-\uDE8B]|\uD83A[\uDD5E\uDD5F]/
 });
-var bs = W((D4, gs) => {
+var xs = W((H4, ys) => {
     "use strict";
-    var fs = {};
+    var bs = {};
 
-    function vd(r) {
-        var e, i, a = fs[r];
+    function Sd(r) {
+        var e, i, a = bs[r];
         if (a) return a;
-        for (a = fs[r] = [], e = 0; e < 128; e++) i = String.fromCharCode(e), /^[0-9a-z]$/i.test(i) ? a.push(i) : a.push("%" + ("0" + e.toString(16).toUpperCase()).slice(-2));
+        for (a = bs[r] = [], e = 0; e < 128; e++) i = String.fromCharCode(e), /^[0-9a-z]$/i.test(i) ? a.push(i) : a.push("%" + ("0" + e.toString(16).toUpperCase()).slice(-2));
         for (e = 0; e < r.length; e++) a[r.charCodeAt(e)] = r[e];
         return a
     }
 
-    function T0(r, e, i) {
-        var a, l, c, d, m, g = "";
-        for (typeof e != "string" && (i = e, e = T0.defaultChars), typeof i > "u" && (i = !0), m = vd(e), a = 0, l = r.length; a < l; a++) {
+    function A0(r, e, i) {
+        var a, l, c, d, f, g = "";
+        for (typeof e != "string" && (i = e, e = A0.defaultChars), typeof i > "u" && (i = !0), f = Sd(e), a = 0, l = r.length; a < l; a++) {
             if (c = r.charCodeAt(a), i && c === 37 && a + 2 < l && /^[0-9a-f]{2}$/i.test(r.slice(a + 1, a + 3))) {
                 g += r.slice(a, a + 3), a += 2;
                 continue
             }
             if (c < 128) {
-                g += m[c];
+                g += f[c];
                 continue
             }
             if (c >= 55296 && c <= 57343) {
                 if (c >= 55296 && c <= 56319 && a + 1 < l && (d = r.charCodeAt(a + 1), d >= 56320 && d <= 57343)) {
                     g += encodeURIComponent(r[a] + r[a + 1]), a++;
                     continue
                 }
                 g += "%EF%BF%BD";
                 continue
             }
             g += encodeURIComponent(r[a])
         }
         return g
     }
-    T0.defaultChars = ";/?:@&=+$,-_.!~*'()#";
-    T0.componentChars = "-_.!~*'()";
-    gs.exports = T0
+    A0.defaultChars = ";/?:@&=+$,-_.!~*'()#";
+    A0.componentChars = "-_.!~*'()";
+    ys.exports = A0
 });
-var vs = W((z4, xs) => {
+var ks = W(($4, ws) => {
     "use strict";
-    var ys = {};
+    var vs = {};
 
-    function wd(r) {
-        var e, i, a = ys[r];
+    function Cd(r) {
+        var e, i, a = vs[r];
         if (a) return a;
-        for (a = ys[r] = [], e = 0; e < 128; e++) i = String.fromCharCode(e), a.push(i);
+        for (a = vs[r] = [], e = 0; e < 128; e++) i = String.fromCharCode(e), a.push(i);
         for (e = 0; e < r.length; e++) i = r.charCodeAt(e), a[i] = "%" + ("0" + i.toString(16).toUpperCase()).slice(-2);
         return a
     }
 
-    function A0(r, e) {
+    function q0(r, e) {
         var i;
-        return typeof e != "string" && (e = A0.defaultChars), i = wd(e), r.replace(/(%[a-f0-9]{2})+/gi, function(a) {
-            var l, c, d, m, g, y, _, k = "";
+        return typeof e != "string" && (e = q0.defaultChars), i = Cd(e), r.replace(/(%[a-f0-9]{2})+/gi, function(a) {
+            var l, c, d, f, g, y, _, w = "";
             for (l = 0, c = a.length; l < c; l += 3) {
                 if (d = parseInt(a.slice(l + 1, l + 3), 16), d < 128) {
-                    k += i[d];
+                    w += i[d];
                     continue
                 }
-                if ((d & 224) === 192 && l + 3 < c && (m = parseInt(a.slice(l + 4, l + 6), 16), (m & 192) === 128)) {
-                    _ = d << 6 & 1984 | m & 63, _ < 128 ? k += "\uFFFD\uFFFD" : k += String.fromCharCode(_), l += 3;
+                if ((d & 224) === 192 && l + 3 < c && (f = parseInt(a.slice(l + 4, l + 6), 16), (f & 192) === 128)) {
+                    _ = d << 6 & 1984 | f & 63, _ < 128 ? w += "\uFFFD\uFFFD" : w += String.fromCharCode(_), l += 3;
                     continue
                 }
-                if ((d & 240) === 224 && l + 6 < c && (m = parseInt(a.slice(l + 4, l + 6), 16), g = parseInt(a.slice(l + 7, l + 9), 16), (m & 192) === 128 && (g & 192) === 128)) {
-                    _ = d << 12 & 61440 | m << 6 & 4032 | g & 63, _ < 2048 || _ >= 55296 && _ <= 57343 ? k += "\uFFFD\uFFFD\uFFFD" : k += String.fromCharCode(_), l += 6;
+                if ((d & 240) === 224 && l + 6 < c && (f = parseInt(a.slice(l + 4, l + 6), 16), g = parseInt(a.slice(l + 7, l + 9), 16), (f & 192) === 128 && (g & 192) === 128)) {
+                    _ = d << 12 & 61440 | f << 6 & 4032 | g & 63, _ < 2048 || _ >= 55296 && _ <= 57343 ? w += "\uFFFD\uFFFD\uFFFD" : w += String.fromCharCode(_), l += 6;
                     continue
                 }
-                if ((d & 248) === 240 && l + 9 < c && (m = parseInt(a.slice(l + 4, l + 6), 16), g = parseInt(a.slice(l + 7, l + 9), 16), y = parseInt(a.slice(l + 10, l + 12), 16), (m & 192) === 128 && (g & 192) === 128 && (y & 192) === 128)) {
-                    _ = d << 18 & 1835008 | m << 12 & 258048 | g << 6 & 4032 | y & 63, _ < 65536 || _ > 1114111 ? k += "\uFFFD\uFFFD\uFFFD\uFFFD" : (_ -= 65536, k += String.fromCharCode(55296 + (_ >> 10), 56320 + (_ & 1023))), l += 9;
+                if ((d & 248) === 240 && l + 9 < c && (f = parseInt(a.slice(l + 4, l + 6), 16), g = parseInt(a.slice(l + 7, l + 9), 16), y = parseInt(a.slice(l + 10, l + 12), 16), (f & 192) === 128 && (g & 192) === 128 && (y & 192) === 128)) {
+                    _ = d << 18 & 1835008 | f << 12 & 258048 | g << 6 & 4032 | y & 63, _ < 65536 || _ > 1114111 ? w += "\uFFFD\uFFFD\uFFFD\uFFFD" : (_ -= 65536, w += String.fromCharCode(55296 + (_ >> 10), 56320 + (_ & 1023))), l += 9;
                     continue
                 }
-                k += "\uFFFD"
+                w += "\uFFFD"
             }
-            return k
+            return w
         })
     }
-    A0.defaultChars = ";/?:@&=+$,#";
-    A0.componentChars = "";
-    xs.exports = A0
+    q0.defaultChars = ";/?:@&=+$,#";
+    q0.componentChars = "";
+    ws.exports = q0
 });
-var ks = W((R4, ws) => {
+var Ss = W((G4, _s) => {
     "use strict";
-    ws.exports = function(e) {
+    _s.exports = function(e) {
         var i = "";
         return i += e.protocol || "", i += e.slashes ? "//" : "", i += e.auth ? e.auth + "@" : "", e.hostname && e.hostname.indexOf(":") !== -1 ? i += "[" + e.hostname + "]" : i += e.hostname || "", i += e.port ? ":" + e.port : "", i += e.pathname || "", i += e.search || "", i += e.hash || "", i
     }
 });
-var Ms = W((F4, qs) => {
+var Ds = W((V4, Es) => {
     "use strict";
 
-    function q0() {
+    function M0() {
         this.protocol = null, this.slashes = null, this.auth = null, this.port = null, this.hostname = null, this.hash = null, this.search = null, this.pathname = null
     }
-    var kd = /^([a-z0-9.+-]+:)/i,
-        _d = /:[0-9]*$/,
-        Sd = /^(\/\/?(?!\/)[^\?\s]*)(\?[^\s]*)?$/,
-        Cd = ["<", ">", '"', "`", " ", "\r", `
+    var Td = /^([a-z0-9.+-]+:)/i,
+        Ad = /:[0-9]*$/,
+        qd = /^(\/\/?(?!\/)[^\?\s]*)(\?[^\s]*)?$/,
+        Md = ["<", ">", '"', "`", " ", "\r", `
 `, "	"],
-        Td = ["{", "}", "|", "\\", "^", "`"].concat(Cd),
-        Ad = ["'"].concat(Td),
-        _s = ["%", "/", "?", ";", "#"].concat(Ad),
-        Ss = ["/", "?", "#"],
-        qd = 255,
-        Cs = /^[+a-z0-9A-Z_-]{0,63}$/,
-        Md = /^([+a-z0-9A-Z_-]{0,63})(.*)$/,
-        Ts = {
+        Ed = ["{", "}", "|", "\\", "^", "`"].concat(Md),
+        Dd = ["'"].concat(Ed),
+        Cs = ["%", "/", "?", ";", "#"].concat(Dd),
+        Ts = ["/", "?", "#"],
+        zd = 255,
+        As = /^[+a-z0-9A-Z_-]{0,63}$/,
+        Rd = /^([+a-z0-9A-Z_-]{0,63})(.*)$/,
+        qs = {
             javascript: !0,
             "javascript:": !0
         },
-        As = {
+        Ms = {
             http: !0,
             https: !0,
             ftp: !0,
             gopher: !0,
             file: !0,
             "http:": !0,
             "https:": !0,
             "ftp:": !0,
             "gopher:": !0,
             "file:": !0
         };
 
-    function Ed(r, e) {
-        if (r && r instanceof q0) return r;
-        var i = new q0;
+    function Fd(r, e) {
+        if (r && r instanceof M0) return r;
+        var i = new M0;
         return i.parse(r, e), i
     }
-    q0.prototype.parse = function(r, e) {
-        var i, a, l, c, d, m = r;
-        if (m = m.trim(), !e && r.split("#").length === 1) {
-            var g = Sd.exec(m);
+    M0.prototype.parse = function(r, e) {
+        var i, a, l, c, d, f = r;
+        if (f = f.trim(), !e && r.split("#").length === 1) {
+            var g = qd.exec(f);
             if (g) return this.pathname = g[1], g[2] && (this.search = g[2]), this
         }
-        var y = kd.exec(m);
-        if (y && (y = y[0], l = y.toLowerCase(), this.protocol = y, m = m.substr(y.length)), (e || y || m.match(/^\/\/[^@\/]+@[^@\/]+/)) && (d = m.substr(0, 2) === "//", d && !(y && Ts[y]) && (m = m.substr(2), this.slashes = !0)), !Ts[y] && (d || y && !As[y])) {
+        var y = Td.exec(f);
+        if (y && (y = y[0], l = y.toLowerCase(), this.protocol = y, f = f.substr(y.length)), (e || y || f.match(/^\/\/[^@\/]+@[^@\/]+/)) && (d = f.substr(0, 2) === "//", d && !(y && qs[y]) && (f = f.substr(2), this.slashes = !0)), !qs[y] && (d || y && !Ms[y])) {
             var _ = -1;
-            for (i = 0; i < Ss.length; i++) c = m.indexOf(Ss[i]), c !== -1 && (_ === -1 || c < _) && (_ = c);
-            var k, T;
-            for (_ === -1 ? T = m.lastIndexOf("@") : T = m.lastIndexOf("@", _), T !== -1 && (k = m.slice(0, T), m = m.slice(T + 1), this.auth = k), _ = -1, i = 0; i < _s.length; i++) c = m.indexOf(_s[i]), c !== -1 && (_ === -1 || c < _) && (_ = c);
-            _ === -1 && (_ = m.length), m[_ - 1] === ":" && _--;
-            var A = m.slice(0, _);
-            m = m.slice(_), this.parseHost(A), this.hostname = this.hostname || "";
+            for (i = 0; i < Ts.length; i++) c = f.indexOf(Ts[i]), c !== -1 && (_ === -1 || c < _) && (_ = c);
+            var w, T;
+            for (_ === -1 ? T = f.lastIndexOf("@") : T = f.lastIndexOf("@", _), T !== -1 && (w = f.slice(0, T), f = f.slice(T + 1), this.auth = w), _ = -1, i = 0; i < Cs.length; i++) c = f.indexOf(Cs[i]), c !== -1 && (_ === -1 || c < _) && (_ = c);
+            _ === -1 && (_ = f.length), f[_ - 1] === ":" && _--;
+            var A = f.slice(0, _);
+            f = f.slice(_), this.parseHost(A), this.hostname = this.hostname || "";
             var L = this.hostname[0] === "[" && this.hostname[this.hostname.length - 1] === "]";
             if (!L) {
                 var R = this.hostname.split(/\./);
                 for (i = 0, a = R.length; i < a; i++) {
-                    var G = R[i];
-                    if (G && !G.match(Cs)) {
-                        for (var P = "", I = 0, Y = G.length; I < Y; I++) G.charCodeAt(I) > 127 ? P += "x" : P += G[I];
-                        if (!P.match(Cs)) {
+                    var O = R[i];
+                    if (O && !O.match(As)) {
+                        for (var P = "", I = 0, Y = O.length; I < Y; I++) O.charCodeAt(I) > 127 ? P += "x" : P += O[I];
+                        if (!P.match(As)) {
                             var re = R.slice(0, i),
                                 te = R.slice(i + 1),
-                                j = G.match(Md);
-                            j && (re.push(j[1]), te.unshift(j[2])), te.length && (m = te.join(".") + m), this.hostname = re.join(".");
+                                j = O.match(Rd);
+                            j && (re.push(j[1]), te.unshift(j[2])), te.length && (f = te.join(".") + f), this.hostname = re.join(".");
                             break
                         }
                     }
                 }
             }
-            this.hostname.length > qd && (this.hostname = ""), L && (this.hostname = this.hostname.substr(1, this.hostname.length - 2))
+            this.hostname.length > zd && (this.hostname = ""), L && (this.hostname = this.hostname.substr(1, this.hostname.length - 2))
         }
-        var ne = m.indexOf("#");
-        ne !== -1 && (this.hash = m.substr(ne), m = m.slice(0, ne));
-        var pe = m.indexOf("?");
-        return pe !== -1 && (this.search = m.substr(pe), m = m.slice(0, pe)), m && (this.pathname = m), As[l] && this.hostname && !this.pathname && (this.pathname = ""), this
+        var ne = f.indexOf("#");
+        ne !== -1 && (this.hash = f.substr(ne), f = f.slice(0, ne));
+        var pe = f.indexOf("?");
+        return pe !== -1 && (this.search = f.substr(pe), f = f.slice(0, pe)), f && (this.pathname = f), Ms[l] && this.hostname && !this.pathname && (this.pathname = ""), this
     };
-    q0.prototype.parseHost = function(r) {
-        var e = _d.exec(r);
+    M0.prototype.parseHost = function(r) {
+        var e = Ad.exec(r);
         e && (e = e[0], e !== ":" && (this.port = e.substr(1)), r = r.substr(0, r.length - e.length)), r && (this.hostname = r)
     };
-    qs.exports = Ed
+    Es.exports = Fd
 });
-var ei = W((B4, Nr) => {
+var ii = W((j4, Nr) => {
     "use strict";
-    Nr.exports.encode = bs();
-    Nr.exports.decode = vs();
-    Nr.exports.format = ks();
-    Nr.exports.parse = Ms()
+    Nr.exports.encode = xs();
+    Nr.exports.decode = ks();
+    Nr.exports.format = Ss();
+    Nr.exports.parse = Ds()
 });
-var ti = W((N4, Es) => {
-    Es.exports = /[\0-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF]/
+var oi = W((U4, zs) => {
+    zs.exports = /[\0-\uD7FF\uE000-\uFFFF]|[\uD800-\uDBFF][\uDC00-\uDFFF]|[\uD800-\uDBFF](?![\uDC00-\uDFFF])|(?:[^\uD800-\uDBFF]|^)[\uDC00-\uDFFF]/
 });
-var ri = W((L4, Ds) => {
-    Ds.exports = /[\0-\x1F\x7F-\x9F]/
+var ai = W((W4, Rs) => {
+    Rs.exports = /[\0-\x1F\x7F-\x9F]/
 });
-var Rs = W((P4, zs) => {
-    zs.exports = /[\xAD\u0600-\u0605\u061C\u06DD\u070F\u08E2\u180E\u200B-\u200F\u202A-\u202E\u2060-\u2064\u2066-\u206F\uFEFF\uFFF9-\uFFFB]|\uD804[\uDCBD\uDCCD]|\uD82F[\uDCA0-\uDCA3]|\uD834[\uDD73-\uDD7A]|\uDB40[\uDC01\uDC20-\uDC7F]/
+var Bs = W((Y4, Fs) => {
+    Fs.exports = /[\xAD\u0600-\u0605\u061C\u06DD\u070F\u08E2\u180E\u200B-\u200F\u202A-\u202E\u2060-\u2064\u2066-\u206F\uFEFF\uFFF9-\uFFFB]|\uD804[\uDCBD\uDCCD]|\uD82F[\uDCA0-\uDCA3]|\uD834[\uDD73-\uDD7A]|\uDB40[\uDC01\uDC20-\uDC7F]/
 });
-var ni = W((I4, Fs) => {
-    Fs.exports = /[ \xA0\u1680\u2000-\u200A\u2028\u2029\u202F\u205F\u3000]/
+var si = W((Z4, Ns) => {
+    Ns.exports = /[ \xA0\u1680\u2000-\u200A\u2028\u2029\u202F\u205F\u3000]/
 });
-var Bs = W(pr => {
+var Ls = W(pr => {
     "use strict";
-    pr.Any = ti();
-    pr.Cc = ri();
-    pr.Cf = Rs();
-    pr.P = C0();
-    pr.Z = ni()
+    pr.Any = oi();
+    pr.Cc = ai();
+    pr.Cf = Bs();
+    pr.P = T0();
+    pr.Z = si()
 });
-var Se = W(Je => {
+var Se = W(Ke => {
     "use strict";
 
-    function Dd(r) {
+    function Bd(r) {
         return Object.prototype.toString.call(r)
     }
 
-    function zd(r) {
-        return Dd(r) === "[object String]"
+    function Nd(r) {
+        return Bd(r) === "[object String]"
     }
-    var Rd = Object.prototype.hasOwnProperty;
+    var Ld = Object.prototype.hasOwnProperty;
 
-    function Ls(r, e) {
-        return Rd.call(r, e)
+    function Is(r, e) {
+        return Ld.call(r, e)
     }
 
-    function Fd(r) {
+    function Pd(r) {
         var e = Array.prototype.slice.call(arguments, 1);
         return e.forEach(function(i) {
             if (i) {
                 if (typeof i != "object") throw new TypeError(i + "must be object");
                 Object.keys(i).forEach(function(a) {
                     r[a] = i[a]
                 })
             }
         }), r
     }
 
-    function Bd(r, e, i) {
+    function Id(r, e, i) {
         return [].concat(r.slice(0, e), i, r.slice(e + 1))
     }
 
-    function Ps(r) {
+    function Os(r) {
         return !(r >= 55296 && r <= 57343 || r >= 64976 && r <= 65007 || (r & 65535) === 65535 || (r & 65535) === 65534 || r >= 0 && r <= 8 || r === 11 || r >= 14 && r <= 31 || r >= 127 && r <= 159 || r > 1114111)
     }
 
-    function Is(r) {
+    function Hs(r) {
         if (r > 65535) {
             r -= 65536;
             var e = 55296 + (r >> 10),
                 i = 56320 + (r & 1023);
             return String.fromCharCode(e, i)
         }
         return String.fromCharCode(r)
     }
-    var Os = /\\([!"#$%&'()*+,\-.\/:;<=>?@[\\\]^_`{|}~])/g,
-        Nd = /&([a-z#][a-z0-9]{1,31});/gi,
-        Ld = new RegExp(Os.source + "|" + Nd.source, "gi"),
-        Pd = /^#((?:x[a-f0-9]{1,8}|[0-9]{1,8}))$/i,
-        Ns = Kn();
+    var $s = /\\([!"#$%&'()*+,\-.\/:;<=>?@[\\\]^_`{|}~])/g,
+        Od = /&([a-z#][a-z0-9]{1,31});/gi,
+        Hd = new RegExp($s.source + "|" + Od.source, "gi"),
+        $d = /^#((?:x[a-f0-9]{1,8}|[0-9]{1,8}))$/i,
+        Ps = ni();
 
-    function Id(r, e) {
+    function Gd(r, e) {
         var i;
-        return Ls(Ns, e) ? Ns[e] : e.charCodeAt(0) === 35 && Pd.test(e) && (i = e[1].toLowerCase() === "x" ? parseInt(e.slice(2), 16) : parseInt(e.slice(1), 10), Ps(i)) ? Is(i) : r
+        return Is(Ps, e) ? Ps[e] : e.charCodeAt(0) === 35 && $d.test(e) && (i = e[1].toLowerCase() === "x" ? parseInt(e.slice(2), 16) : parseInt(e.slice(1), 10), Os(i)) ? Hs(i) : r
     }
 
-    function Od(r) {
-        return r.indexOf("\\") < 0 ? r : r.replace(Os, "$1")
+    function Vd(r) {
+        return r.indexOf("\\") < 0 ? r : r.replace($s, "$1")
     }
 
-    function Hd(r) {
-        return r.indexOf("\\") < 0 && r.indexOf("&") < 0 ? r : r.replace(Ld, function(e, i, a) {
-            return i || Id(e, a)
+    function jd(r) {
+        return r.indexOf("\\") < 0 && r.indexOf("&") < 0 ? r : r.replace(Hd, function(e, i, a) {
+            return i || Gd(e, a)
         })
     }
-    var $d = /[&<>"]/,
-        Gd = /[&<>"]/g,
-        Vd = {
+    var Ud = /[&<>"]/,
+        Wd = /[&<>"]/g,
+        Yd = {
             "&": "&amp;",
             "<": "&lt;",
             ">": "&gt;",
             '"': "&quot;"
         };
 
-    function jd(r) {
-        return Vd[r]
+    function Zd(r) {
+        return Yd[r]
     }
 
-    function Ud(r) {
-        return $d.test(r) ? r.replace(Gd, jd) : r
+    function Qd(r) {
+        return Ud.test(r) ? r.replace(Wd, Zd) : r
     }
-    var Wd = /[.?*+^$[\]\\(){}|-]/g;
+    var Xd = /[.?*+^$[\]\\(){}|-]/g;
 
-    function Yd(r) {
-        return r.replace(Wd, "\\$&")
+    function Jd(r) {
+        return r.replace(Xd, "\\$&")
     }
 
-    function Qd(r) {
+    function Kd(r) {
         switch (r) {
             case 9:
             case 32:
                 return !0
         }
         return !1
     }
 
-    function Zd(r) {
+    function em(r) {
         if (r >= 8192 && r <= 8202) return !0;
         switch (r) {
             case 9:
             case 10:
             case 11:
             case 12:
             case 13:
@@ -3677,21 +3677,21 @@
             case 8239:
             case 8287:
             case 12288:
                 return !0
         }
         return !1
     }
-    var Xd = C0();
+    var tm = T0();
 
-    function Jd(r) {
-        return Xd.test(r)
+    function rm(r) {
+        return tm.test(r)
     }
 
-    function Kd(r) {
+    function nm(r) {
         switch (r) {
             case 33:
             case 34:
             case 35:
             case 36:
             case 37:
             case 38:
@@ -3723,144 +3723,144 @@
             case 126:
                 return !0;
             default:
                 return !1
         }
     }
 
-    function em(r) {
+    function im(r) {
         return r = r.trim().replace(/\s+/g, " "), "\u1E9E".toLowerCase() === "\u1E7E" && (r = r.replace(/ẞ/g, "\xDF")), r.toLowerCase().toUpperCase()
     }
-    Je.lib = {};
-    Je.lib.mdurl = ei();
-    Je.lib.ucmicro = Bs();
-    Je.assign = Fd;
-    Je.isString = zd;
-    Je.has = Ls;
-    Je.unescapeMd = Od;
-    Je.unescapeAll = Hd;
-    Je.isValidEntityCode = Ps;
-    Je.fromCodePoint = Is;
-    Je.escapeHtml = Ud;
-    Je.arrayReplaceAt = Bd;
-    Je.isSpace = Qd;
-    Je.isWhiteSpace = Zd;
-    Je.isMdAsciiPunct = Kd;
-    Je.isPunctChar = Jd;
-    Je.escapeRE = Yd;
-    Je.normalizeReference = em
+    Ke.lib = {};
+    Ke.lib.mdurl = ii();
+    Ke.lib.ucmicro = Ls();
+    Ke.assign = Pd;
+    Ke.isString = Nd;
+    Ke.has = Is;
+    Ke.unescapeMd = Vd;
+    Ke.unescapeAll = jd;
+    Ke.isValidEntityCode = Os;
+    Ke.fromCodePoint = Hs;
+    Ke.escapeHtml = Qd;
+    Ke.arrayReplaceAt = Id;
+    Ke.isSpace = Kd;
+    Ke.isWhiteSpace = em;
+    Ke.isMdAsciiPunct = nm;
+    Ke.isPunctChar = rm;
+    Ke.escapeRE = Jd;
+    Ke.normalizeReference = im
 });
-var $s = W(($4, Hs) => {
+var Vs = W((J4, Gs) => {
     "use strict";
-    Hs.exports = function(e, i, a) {
-        var l, c, d, m, g = -1,
+    Gs.exports = function(e, i, a) {
+        var l, c, d, f, g = -1,
             y = e.posMax,
             _ = e.pos;
         for (e.pos = i + 1, l = 1; e.pos < y;) {
             if (d = e.src.charCodeAt(e.pos), d === 93 && (l--, l === 0)) {
                 c = !0;
                 break
             }
-            if (m = e.pos, e.md.inline.skipToken(e), d === 91) {
-                if (m === e.pos - 1) l++;
+            if (f = e.pos, e.md.inline.skipToken(e), d === 91) {
+                if (f === e.pos - 1) l++;
                 else if (a) return e.pos = _, -1
             }
         }
         return c && (g = e.pos), e.pos = _, g
     }
 });
-var js = W((G4, Vs) => {
+var Ws = W((K4, Us) => {
     "use strict";
-    var Gs = Se().unescapeAll;
-    Vs.exports = function(e, i, a) {
+    var js = Se().unescapeAll;
+    Us.exports = function(e, i, a) {
         var l, c, d = i,
-            m = {
+            f = {
                 ok: !1,
                 pos: 0,
                 lines: 0,
                 str: ""
             };
         if (e.charCodeAt(d) === 60) {
             for (d++; d < a;) {
-                if (l = e.charCodeAt(d), l === 10 || l === 60) return m;
-                if (l === 62) return m.pos = d + 1, m.str = Gs(e.slice(i + 1, d)), m.ok = !0, m;
+                if (l = e.charCodeAt(d), l === 10 || l === 60) return f;
+                if (l === 62) return f.pos = d + 1, f.str = js(e.slice(i + 1, d)), f.ok = !0, f;
                 if (l === 92 && d + 1 < a) {
                     d += 2;
                     continue
                 }
                 d++
             }
-            return m
+            return f
         }
         for (c = 0; d < a && (l = e.charCodeAt(d), !(l === 32 || l < 32 || l === 127));) {
             if (l === 92 && d + 1 < a) {
                 if (e.charCodeAt(d + 1) === 32) break;
                 d += 2;
                 continue
             }
-            if (l === 40 && (c++, c > 32)) return m;
+            if (l === 40 && (c++, c > 32)) return f;
             if (l === 41) {
                 if (c === 0) break;
                 c--
             }
             d++
         }
-        return i === d || c !== 0 || (m.str = Gs(e.slice(i, d)), m.pos = d, m.ok = !0), m
+        return i === d || c !== 0 || (f.str = js(e.slice(i, d)), f.pos = d, f.ok = !0), f
     }
 });
-var Ws = W((V4, Us) => {
+var Zs = W((e2, Ys) => {
     "use strict";
-    var tm = Se().unescapeAll;
-    Us.exports = function(e, i, a) {
+    var om = Se().unescapeAll;
+    Ys.exports = function(e, i, a) {
         var l, c, d = 0,
-            m = i,
+            f = i,
             g = {
                 ok: !1,
                 pos: 0,
                 lines: 0,
                 str: ""
             };
-        if (m >= a || (c = e.charCodeAt(m), c !== 34 && c !== 39 && c !== 40)) return g;
-        for (m++, c === 40 && (c = 41); m < a;) {
-            if (l = e.charCodeAt(m), l === c) return g.pos = m + 1, g.lines = d, g.str = tm(e.slice(i + 1, m)), g.ok = !0, g;
+        if (f >= a || (c = e.charCodeAt(f), c !== 34 && c !== 39 && c !== 40)) return g;
+        for (f++, c === 40 && (c = 41); f < a;) {
+            if (l = e.charCodeAt(f), l === c) return g.pos = f + 1, g.lines = d, g.str = om(e.slice(i + 1, f)), g.ok = !0, g;
             if (l === 40 && c === 41) return g;
-            l === 10 ? d++ : l === 92 && m + 1 < a && (m++, e.charCodeAt(m) === 10 && d++), m++
+            l === 10 ? d++ : l === 92 && f + 1 < a && (f++, e.charCodeAt(f) === 10 && d++), f++
         }
         return g
     }
 });
-var Ys = W(M0 => {
+var Qs = W(E0 => {
     "use strict";
-    M0.parseLinkLabel = $s();
-    M0.parseLinkDestination = js();
-    M0.parseLinkTitle = Ws()
+    E0.parseLinkLabel = Vs();
+    E0.parseLinkDestination = Ws();
+    E0.parseLinkTitle = Zs()
 });
-var Zs = W((U4, Qs) => {
+var Js = W((r2, Xs) => {
     "use strict";
-    var rm = Se().assign,
-        nm = Se().unescapeAll,
-        ir = Se().escapeHtml,
+    var am = Se().assign,
+        sm = Se().unescapeAll,
+        or = Se().escapeHtml,
         Ct = {};
     Ct.code_inline = function(r, e, i, a, l) {
         var c = r[e];
-        return "<code" + l.renderAttrs(c) + ">" + ir(c.content) + "</code>"
+        return "<code" + l.renderAttrs(c) + ">" + or(c.content) + "</code>"
     };
     Ct.code_block = function(r, e, i, a, l) {
         var c = r[e];
-        return "<pre" + l.renderAttrs(c) + "><code>" + ir(r[e].content) + `</code></pre>
+        return "<pre" + l.renderAttrs(c) + "><code>" + or(r[e].content) + `</code></pre>
 `
     };
     Ct.fence = function(r, e, i, a, l) {
         var c = r[e],
-            d = c.info ? nm(c.info).trim() : "",
-            m = "",
+            d = c.info ? sm(c.info).trim() : "",
+            f = "",
             g = "",
-            y, _, k, T, A;
-        return d && (k = d.split(/(\s+)/g), m = k[0], g = k.slice(2).join("")), i.highlight ? y = i.highlight(c.content, m, g) || ir(c.content) : y = ir(c.content), y.indexOf("<pre") === 0 ? y + `
-` : d ? (_ = c.attrIndex("class"), T = c.attrs ? c.attrs.slice() : [], _ < 0 ? T.push(["class", i.langPrefix + m]) : (T[_] = T[_].slice(), T[_][1] += " " + i.langPrefix + m), A = {
+            y, _, w, T, A;
+        return d && (w = d.split(/(\s+)/g), f = w[0], g = w.slice(2).join("")), i.highlight ? y = i.highlight(c.content, f, g) || or(c.content) : y = or(c.content), y.indexOf("<pre") === 0 ? y + `
+` : d ? (_ = c.attrIndex("class"), T = c.attrs ? c.attrs.slice() : [], _ < 0 ? T.push(["class", i.langPrefix + f]) : (T[_] = T[_].slice(), T[_][1] += " " + i.langPrefix + f), A = {
             attrs: T
         }, "<pre><code" + l.renderAttrs(A) + ">" + y + `</code></pre>
 `) : "<pre><code" + l.renderAttrs(c) + ">" + y + `</code></pre>
 `
     };
     Ct.image = function(r, e, i, a, l) {
         var c = r[e];
@@ -3874,58 +3874,58 @@
     Ct.softbreak = function(r, e, i) {
         return i.breaks ? i.xhtmlOut ? `<br />
 ` : `<br>
 ` : `
 `
     };
     Ct.text = function(r, e) {
-        return ir(r[e].content)
+        return or(r[e].content)
     };
     Ct.html_block = function(r, e) {
         return r[e].content
     };
     Ct.html_inline = function(r, e) {
         return r[e].content
     };
 
     function fr() {
-        this.rules = rm({}, Ct)
+        this.rules = am({}, Ct)
     }
     fr.prototype.renderAttrs = function(e) {
         var i, a, l;
         if (!e.attrs) return "";
-        for (l = "", i = 0, a = e.attrs.length; i < a; i++) l += " " + ir(e.attrs[i][0]) + '="' + ir(e.attrs[i][1]) + '"';
+        for (l = "", i = 0, a = e.attrs.length; i < a; i++) l += " " + or(e.attrs[i][0]) + '="' + or(e.attrs[i][1]) + '"';
         return l
     };
     fr.prototype.renderToken = function(e, i, a) {
         var l, c = "",
             d = !1,
-            m = e[i];
-        return m.hidden ? "" : (m.block && m.nesting !== -1 && i && e[i - 1].hidden && (c += `
-`), c += (m.nesting === -1 ? "</" : "<") + m.tag, c += this.renderAttrs(m), m.nesting === 0 && a.xhtmlOut && (c += " /"), m.block && (d = !0, m.nesting === 1 && i + 1 < e.length && (l = e[i + 1], (l.type === "inline" || l.hidden || l.nesting === -1 && l.tag === m.tag) && (d = !1))), c += d ? `>
+            f = e[i];
+        return f.hidden ? "" : (f.block && f.nesting !== -1 && i && e[i - 1].hidden && (c += `
+`), c += (f.nesting === -1 ? "</" : "<") + f.tag, c += this.renderAttrs(f), f.nesting === 0 && a.xhtmlOut && (c += " /"), f.block && (d = !0, f.nesting === 1 && i + 1 < e.length && (l = e[i + 1], (l.type === "inline" || l.hidden || l.nesting === -1 && l.tag === f.tag) && (d = !1))), c += d ? `>
 ` : ">", c)
     };
     fr.prototype.renderInline = function(r, e, i) {
-        for (var a, l = "", c = this.rules, d = 0, m = r.length; d < m; d++) a = r[d].type, typeof c[a] < "u" ? l += c[a](r, d, e, i, this) : l += this.renderToken(r, d, e);
+        for (var a, l = "", c = this.rules, d = 0, f = r.length; d < f; d++) a = r[d].type, typeof c[a] < "u" ? l += c[a](r, d, e, i, this) : l += this.renderToken(r, d, e);
         return l
     };
     fr.prototype.renderInlineAsText = function(r, e, i) {
         for (var a = "", l = 0, c = r.length; l < c; l++) r[l].type === "text" ? a += r[l].content : r[l].type === "image" ? a += this.renderInlineAsText(r[l].children, e, i) : r[l].type === "softbreak" && (a += `
 `);
         return a
     };
     fr.prototype.render = function(r, e, i) {
         var a, l, c, d = "",
-            m = this.rules;
-        for (a = 0, l = r.length; a < l; a++) c = r[a].type, c === "inline" ? d += this.renderInline(r[a].children, e, i) : typeof m[c] < "u" ? d += m[c](r, a, e, i, this) : d += this.renderToken(r, a, e, i);
+            f = this.rules;
+        for (a = 0, l = r.length; a < l; a++) c = r[a].type, c === "inline" ? d += this.renderInline(r[a].children, e, i) : typeof f[c] < "u" ? d += f[c](r, a, e, i, this) : d += this.renderToken(r, a, e, i);
         return d
     };
-    Qs.exports = fr
+    Xs.exports = fr
 });
-var E0 = W((W4, Xs) => {
+var D0 = W((n2, Ks) => {
     "use strict";
 
     function xt() {
         this.__rules__ = [], this.__cache__ = null
     }
     xt.prototype.__find__ = function(r) {
         for (var e = 0; e < this.__rules__.length; e++)
@@ -4010,175 +4010,175 @@
             }
             this.__rules__[l].enabled = !1, i.push(a)
         }, this), this.__cache__ = null, i
     };
     xt.prototype.getRules = function(r) {
         return this.__cache__ === null && this.__compile__(), this.__cache__[r] || []
     };
-    Xs.exports = xt
+    Ks.exports = xt
 });
-var Ks = W((Y4, Js) => {
+var tl = W((i2, el) => {
     "use strict";
-    var im = /\r\n?|\n/g,
-        om = /\0/g;
-    Js.exports = function(e) {
+    var lm = /\r\n?|\n/g,
+        cm = /\0/g;
+    el.exports = function(e) {
         var i;
-        i = e.src.replace(im, `
-`), i = i.replace(om, "\uFFFD"), e.src = i
+        i = e.src.replace(lm, `
+`), i = i.replace(cm, "\uFFFD"), e.src = i
     }
 });
-var tl = W((Q4, el) => {
+var nl = W((o2, rl) => {
     "use strict";
-    el.exports = function(e) {
+    rl.exports = function(e) {
         var i;
         e.inlineMode ? (i = new e.Token("inline", "", 0), i.content = e.src, i.map = [0, 1], i.children = [], e.tokens.push(i)) : e.md.block.parse(e.src, e.md, e.env, e.tokens)
     }
 });
-var nl = W((Z4, rl) => {
+var ol = W((a2, il) => {
     "use strict";
-    rl.exports = function(e) {
+    il.exports = function(e) {
         var i = e.tokens,
             a, l, c;
         for (l = 0, c = i.length; l < c; l++) a = i[l], a.type === "inline" && e.md.inline.parse(a.content, e.md, e.env, a.children)
     }
 });
-var ol = W((X4, il) => {
+var sl = W((s2, al) => {
     "use strict";
-    var am = Se().arrayReplaceAt;
+    var um = Se().arrayReplaceAt;
 
-    function sm(r) {
+    function hm(r) {
         return /^<a[>\s]/i.test(r)
     }
 
-    function lm(r) {
+    function dm(r) {
         return /^<\/a\s*>/i.test(r)
     }
-    il.exports = function(e) {
-        var i, a, l, c, d, m, g, y, _, k, T, A, L, R, G, P, I = e.tokens,
+    al.exports = function(e) {
+        var i, a, l, c, d, f, g, y, _, w, T, A, L, R, O, P, I = e.tokens,
             Y;
         if (e.md.options.linkify) {
             for (a = 0, l = I.length; a < l; a++)
                 if (!(I[a].type !== "inline" || !e.md.linkify.pretest(I[a].content)))
                     for (c = I[a].children, L = 0, i = c.length - 1; i >= 0; i--) {
-                        if (m = c[i], m.type === "link_close") {
-                            for (i--; c[i].level !== m.level && c[i].type !== "link_open";) i--;
+                        if (f = c[i], f.type === "link_close") {
+                            for (i--; c[i].level !== f.level && c[i].type !== "link_open";) i--;
                             continue
                         }
-                        if (m.type === "html_inline" && (sm(m.content) && L > 0 && L--, lm(m.content) && L++), !(L > 0) && m.type === "text" && e.md.linkify.test(m.content)) {
-                            for (_ = m.content, Y = e.md.linkify.match(_), g = [], A = m.level, T = 0, Y.length > 0 && Y[0].index === 0 && i > 0 && c[i - 1].type === "text_special" && (Y = Y.slice(1)), y = 0; y < Y.length; y++) R = Y[y].url, G = e.md.normalizeLink(R), e.md.validateLink(G) && (P = Y[y].text, Y[y].schema ? Y[y].schema === "mailto:" && !/^mailto:/i.test(P) ? P = e.md.normalizeLinkText("mailto:" + P).replace(/^mailto:/, "") : P = e.md.normalizeLinkText(P) : P = e.md.normalizeLinkText("http://" + P).replace(/^http:\/\//, ""), k = Y[y].index, k > T && (d = new e.Token("text", "", 0), d.content = _.slice(T, k), d.level = A, g.push(d)), d = new e.Token("link_open", "a", 1), d.attrs = [
-                                ["href", G]
+                        if (f.type === "html_inline" && (hm(f.content) && L > 0 && L--, dm(f.content) && L++), !(L > 0) && f.type === "text" && e.md.linkify.test(f.content)) {
+                            for (_ = f.content, Y = e.md.linkify.match(_), g = [], A = f.level, T = 0, Y.length > 0 && Y[0].index === 0 && i > 0 && c[i - 1].type === "text_special" && (Y = Y.slice(1)), y = 0; y < Y.length; y++) R = Y[y].url, O = e.md.normalizeLink(R), e.md.validateLink(O) && (P = Y[y].text, Y[y].schema ? Y[y].schema === "mailto:" && !/^mailto:/i.test(P) ? P = e.md.normalizeLinkText("mailto:" + P).replace(/^mailto:/, "") : P = e.md.normalizeLinkText(P) : P = e.md.normalizeLinkText("http://" + P).replace(/^http:\/\//, ""), w = Y[y].index, w > T && (d = new e.Token("text", "", 0), d.content = _.slice(T, w), d.level = A, g.push(d)), d = new e.Token("link_open", "a", 1), d.attrs = [
+                                ["href", O]
                             ], d.level = A++, d.markup = "linkify", d.info = "auto", g.push(d), d = new e.Token("text", "", 0), d.content = P, d.level = A, g.push(d), d = new e.Token("link_close", "a", -1), d.level = --A, d.markup = "linkify", d.info = "auto", g.push(d), T = Y[y].lastIndex);
-                            T < _.length && (d = new e.Token("text", "", 0), d.content = _.slice(T), d.level = A, g.push(d)), I[a].children = c = am(c, i, g)
+                            T < _.length && (d = new e.Token("text", "", 0), d.content = _.slice(T), d.level = A, g.push(d)), I[a].children = c = um(c, i, g)
                         }
                     }
         }
     }
 });
-var ll = W((J4, sl) => {
+var ul = W((l2, cl) => {
     "use strict";
-    var al = /\+-|\.\.|\?\?\?\?|!!!!|,,|--/,
-        cm = /\((c|tm|r)\)/i,
-        um = /\((c|tm|r)\)/ig,
-        hm = {
+    var ll = /\+-|\.\.|\?\?\?\?|!!!!|,,|--/,
+        mm = /\((c|tm|r)\)/i,
+        pm = /\((c|tm|r)\)/ig,
+        fm = {
             c: "\xA9",
             r: "\xAE",
             tm: "\u2122"
         };
 
-    function dm(r, e) {
-        return hm[e.toLowerCase()]
+    function gm(r, e) {
+        return fm[e.toLowerCase()]
     }
 
-    function mm(r) {
+    function bm(r) {
         var e, i, a = 0;
-        for (e = r.length - 1; e >= 0; e--) i = r[e], i.type === "text" && !a && (i.content = i.content.replace(um, dm)), i.type === "link_open" && i.info === "auto" && a--, i.type === "link_close" && i.info === "auto" && a++
+        for (e = r.length - 1; e >= 0; e--) i = r[e], i.type === "text" && !a && (i.content = i.content.replace(pm, gm)), i.type === "link_open" && i.info === "auto" && a--, i.type === "link_close" && i.info === "auto" && a++
     }
 
-    function pm(r) {
+    function ym(r) {
         var e, i, a = 0;
-        for (e = r.length - 1; e >= 0; e--) i = r[e], i.type === "text" && !a && al.test(i.content) && (i.content = i.content.replace(/\+-/g, "\xB1").replace(/\.{2,}/g, "\u2026").replace(/([?!])…/g, "$1..").replace(/([?!]){4,}/g, "$1$1$1").replace(/,{2,}/g, ",").replace(/(^|[^-])---(?=[^-]|$)/mg, "$1\u2014").replace(/(^|\s)--(?=\s|$)/mg, "$1\u2013").replace(/(^|[^-\s])--(?=[^-\s]|$)/mg, "$1\u2013")), i.type === "link_open" && i.info === "auto" && a--, i.type === "link_close" && i.info === "auto" && a++
+        for (e = r.length - 1; e >= 0; e--) i = r[e], i.type === "text" && !a && ll.test(i.content) && (i.content = i.content.replace(/\+-/g, "\xB1").replace(/\.{2,}/g, "\u2026").replace(/([?!])…/g, "$1..").replace(/([?!]){4,}/g, "$1$1$1").replace(/,{2,}/g, ",").replace(/(^|[^-])---(?=[^-]|$)/mg, "$1\u2014").replace(/(^|\s)--(?=\s|$)/mg, "$1\u2013").replace(/(^|[^-\s])--(?=[^-\s]|$)/mg, "$1\u2013")), i.type === "link_open" && i.info === "auto" && a--, i.type === "link_close" && i.info === "auto" && a++
     }
-    sl.exports = function(e) {
+    cl.exports = function(e) {
         var i;
         if (e.md.options.typographer)
-            for (i = e.tokens.length - 1; i >= 0; i--) e.tokens[i].type === "inline" && (cm.test(e.tokens[i].content) && mm(e.tokens[i].children), al.test(e.tokens[i].content) && pm(e.tokens[i].children))
+            for (i = e.tokens.length - 1; i >= 0; i--) e.tokens[i].type === "inline" && (mm.test(e.tokens[i].content) && bm(e.tokens[i].children), ll.test(e.tokens[i].content) && ym(e.tokens[i].children))
     }
 });
-var fl = W((K4, pl) => {
+var bl = W((c2, gl) => {
     "use strict";
-    var cl = Se().isWhiteSpace,
-        ul = Se().isPunctChar,
-        hl = Se().isMdAsciiPunct,
-        fm = /['"]/,
-        dl = /['"]/g,
-        ml = "\u2019";
+    var hl = Se().isWhiteSpace,
+        dl = Se().isPunctChar,
+        ml = Se().isMdAsciiPunct,
+        xm = /['"]/,
+        pl = /['"]/g,
+        fl = "\u2019";
 
-    function D0(r, e, i) {
+    function z0(r, e, i) {
         return r.slice(0, e) + i + r.slice(e + 1)
     }
 
-    function gm(r, e) {
-        var i, a, l, c, d, m, g, y, _, k, T, A, L, R, G, P, I, Y, re, te, j;
+    function vm(r, e) {
+        var i, a, l, c, d, f, g, y, _, w, T, A, L, R, O, P, I, Y, re, te, j;
         for (re = [], i = 0; i < r.length; i++) {
             for (a = r[i], g = r[i].level, I = re.length - 1; I >= 0 && !(re[I].level <= g); I--);
             if (re.length = I + 1, a.type === "text") {
-                l = a.content, d = 0, m = l.length;
-                e: for (; d < m && (dl.lastIndex = d, c = dl.exec(l), !!c);) {
-                    if (G = P = !0, d = c.index + 1, Y = c[0] === "'", _ = 32, c.index - 1 >= 0) _ = l.charCodeAt(c.index - 1);
+                l = a.content, d = 0, f = l.length;
+                e: for (; d < f && (pl.lastIndex = d, c = pl.exec(l), !!c);) {
+                    if (O = P = !0, d = c.index + 1, Y = c[0] === "'", _ = 32, c.index - 1 >= 0) _ = l.charCodeAt(c.index - 1);
                     else
                         for (I = i - 1; I >= 0 && !(r[I].type === "softbreak" || r[I].type === "hardbreak"); I--)
                             if (r[I].content) {
                                 _ = r[I].content.charCodeAt(r[I].content.length - 1);
                                 break
-                            } if (k = 32, d < m) k = l.charCodeAt(d);
+                            } if (w = 32, d < f) w = l.charCodeAt(d);
                     else
                         for (I = i + 1; I < r.length && !(r[I].type === "softbreak" || r[I].type === "hardbreak"); I++)
                             if (r[I].content) {
-                                k = r[I].content.charCodeAt(0);
+                                w = r[I].content.charCodeAt(0);
                                 break
-                            } if (T = hl(_) || ul(String.fromCharCode(_)), A = hl(k) || ul(String.fromCharCode(k)), L = cl(_), R = cl(k), R ? G = !1 : A && (L || T || (G = !1)), L ? P = !1 : T && (R || A || (P = !1)), k === 34 && c[0] === '"' && _ >= 48 && _ <= 57 && (P = G = !1), G && P && (G = T, P = A), !G && !P) {
-                        Y && (a.content = D0(a.content, c.index, ml));
+                            } if (T = ml(_) || dl(String.fromCharCode(_)), A = ml(w) || dl(String.fromCharCode(w)), L = hl(_), R = hl(w), R ? O = !1 : A && (L || T || (O = !1)), L ? P = !1 : T && (R || A || (P = !1)), w === 34 && c[0] === '"' && _ >= 48 && _ <= 57 && (P = O = !1), O && P && (O = T, P = A), !O && !P) {
+                        Y && (a.content = z0(a.content, c.index, fl));
                         continue
                     }
                     if (P) {
                         for (I = re.length - 1; I >= 0 && (y = re[I], !(re[I].level < g)); I--)
                             if (y.single === Y && re[I].level === g) {
-                                y = re[I], Y ? (te = e.md.options.quotes[2], j = e.md.options.quotes[3]) : (te = e.md.options.quotes[0], j = e.md.options.quotes[1]), a.content = D0(a.content, c.index, j), r[y.token].content = D0(r[y.token].content, y.pos, te), d += j.length - 1, y.token === i && (d += te.length - 1), l = a.content, m = l.length, re.length = I;
+                                y = re[I], Y ? (te = e.md.options.quotes[2], j = e.md.options.quotes[3]) : (te = e.md.options.quotes[0], j = e.md.options.quotes[1]), a.content = z0(a.content, c.index, j), r[y.token].content = z0(r[y.token].content, y.pos, te), d += j.length - 1, y.token === i && (d += te.length - 1), l = a.content, f = l.length, re.length = I;
                                 continue e
                             }
                     }
-                    G ? re.push({
+                    O ? re.push({
                         token: i,
                         pos: c.index,
                         single: Y,
                         level: g
-                    }) : P && Y && (a.content = D0(a.content, c.index, ml))
+                    }) : P && Y && (a.content = z0(a.content, c.index, fl))
                 }
             }
         }
     }
-    pl.exports = function(e) {
+    gl.exports = function(e) {
         var i;
         if (e.md.options.typographer)
-            for (i = e.tokens.length - 1; i >= 0; i--) e.tokens[i].type !== "inline" || !fm.test(e.tokens[i].content) || gm(e.tokens[i].children, e)
+            for (i = e.tokens.length - 1; i >= 0; i--) e.tokens[i].type !== "inline" || !xm.test(e.tokens[i].content) || vm(e.tokens[i].children, e)
     }
 });
-var bl = W((e2, gl) => {
+var xl = W((u2, yl) => {
     "use strict";
-    gl.exports = function(e) {
-        var i, a, l, c, d, m, g = e.tokens;
+    yl.exports = function(e) {
+        var i, a, l, c, d, f, g = e.tokens;
         for (i = 0, a = g.length; i < a; i++)
             if (g[i].type === "inline") {
                 for (l = g[i].children, d = l.length, c = 0; c < d; c++) l[c].type === "text_special" && (l[c].type = "text");
-                for (c = m = 0; c < d; c++) l[c].type === "text" && c + 1 < d && l[c + 1].type === "text" ? l[c + 1].content = l[c].content + l[c + 1].content : (c !== m && (l[m] = l[c]), m++);
-                c !== m && (l.length = m)
+                for (c = f = 0; c < d; c++) l[c].type === "text" && c + 1 < d && l[c + 1].type === "text" ? l[c + 1].content = l[c].content + l[c + 1].content : (c !== f && (l[f] = l[c]), f++);
+                c !== f && (l.length = f)
             }
     }
 });
-var z0 = W((t2, yl) => {
+var R0 = W((h2, vl) => {
     "use strict";
 
     function gr(r, e, i) {
         this.type = r, this.tag = e, this.attrs = null, this.map = null, this.nesting = i, this.level = 0, this.children = null, this.content = "", this.markup = "", this.info = "", this.meta = null, this.block = !1, this.hidden = !1
     }
     gr.prototype.attrIndex = function(e) {
         var i, a, l;
@@ -4200,107 +4200,107 @@
             a = null;
         return i >= 0 && (a = this.attrs[i][1]), a
     };
     gr.prototype.attrJoin = function(e, i) {
         var a = this.attrIndex(e);
         a < 0 ? this.attrPush([e, i]) : this.attrs[a][1] = this.attrs[a][1] + " " + i
     };
-    yl.exports = gr
+    vl.exports = gr
 });
-var wl = W((r2, vl) => {
+var _l = W((d2, kl) => {
     "use strict";
-    var bm = z0();
+    var wm = R0();
 
-    function xl(r, e, i) {
+    function wl(r, e, i) {
         this.src = r, this.env = i, this.tokens = [], this.inlineMode = !1, this.md = e
     }
-    xl.prototype.Token = bm;
-    vl.exports = xl
+    wl.prototype.Token = wm;
+    kl.exports = wl
 });
-var _l = W((n2, kl) => {
+var Cl = W((m2, Sl) => {
     "use strict";
-    var ym = E0(),
-        ii = [
-            ["normalize", Ks()],
-            ["block", tl()],
-            ["inline", nl()],
-            ["linkify", ol()],
-            ["replacements", ll()],
-            ["smartquotes", fl()],
-            ["text_join", bl()]
+    var km = D0(),
+        li = [
+            ["normalize", tl()],
+            ["block", nl()],
+            ["inline", ol()],
+            ["linkify", sl()],
+            ["replacements", ul()],
+            ["smartquotes", bl()],
+            ["text_join", xl()]
         ];
 
-    function oi() {
-        this.ruler = new ym;
-        for (var r = 0; r < ii.length; r++) this.ruler.push(ii[r][0], ii[r][1])
+    function ci() {
+        this.ruler = new km;
+        for (var r = 0; r < li.length; r++) this.ruler.push(li[r][0], li[r][1])
     }
-    oi.prototype.process = function(r) {
+    ci.prototype.process = function(r) {
         var e, i, a;
         for (a = this.ruler.getRules(""), e = 0, i = a.length; e < i; e++) a[e](r)
     };
-    oi.prototype.State = wl();
-    kl.exports = oi
+    ci.prototype.State = _l();
+    Sl.exports = ci
 });
-var Tl = W((i2, Cl) => {
+var ql = W((p2, Al) => {
     "use strict";
-    var ai = Se().isSpace;
+    var ui = Se().isSpace;
 
-    function si(r, e) {
+    function hi(r, e) {
         var i = r.bMarks[e] + r.tShift[e],
             a = r.eMarks[e];
         return r.src.slice(i, a)
     }
 
-    function Sl(r) {
+    function Tl(r) {
         var e = [],
             i = 0,
             a = r.length,
             l, c = !1,
             d = 0,
-            m = "";
-        for (l = r.charCodeAt(i); i < a;) l === 124 && (c ? (m += r.substring(d, i - 1), d = i) : (e.push(m + r.substring(d, i)), m = "", d = i + 1)), c = l === 92, i++, l = r.charCodeAt(i);
-        return e.push(m + r.substring(d)), e
-    }
-    Cl.exports = function(e, i, a, l) {
-        var c, d, m, g, y, _, k, T, A, L, R, G, P, I, Y, re, te, j;
-        if (i + 2 > a || (_ = i + 1, e.sCount[_] < e.blkIndent) || e.sCount[_] - e.blkIndent >= 4 || (m = e.bMarks[_] + e.tShift[_], m >= e.eMarks[_]) || (te = e.src.charCodeAt(m++), te !== 124 && te !== 45 && te !== 58) || m >= e.eMarks[_] || (j = e.src.charCodeAt(m++), j !== 124 && j !== 45 && j !== 58 && !ai(j)) || te === 45 && ai(j)) return !1;
-        for (; m < e.eMarks[_];) {
-            if (c = e.src.charCodeAt(m), c !== 124 && c !== 45 && c !== 58 && !ai(c)) return !1;
-            m++
-        }
-        for (d = si(e, i + 1), k = d.split("|"), L = [], g = 0; g < k.length; g++) {
-            if (R = k[g].trim(), !R) {
-                if (g === 0 || g === k.length - 1) continue;
+            f = "";
+        for (l = r.charCodeAt(i); i < a;) l === 124 && (c ? (f += r.substring(d, i - 1), d = i) : (e.push(f + r.substring(d, i)), f = "", d = i + 1)), c = l === 92, i++, l = r.charCodeAt(i);
+        return e.push(f + r.substring(d)), e
+    }
+    Al.exports = function(e, i, a, l) {
+        var c, d, f, g, y, _, w, T, A, L, R, O, P, I, Y, re, te, j;
+        if (i + 2 > a || (_ = i + 1, e.sCount[_] < e.blkIndent) || e.sCount[_] - e.blkIndent >= 4 || (f = e.bMarks[_] + e.tShift[_], f >= e.eMarks[_]) || (te = e.src.charCodeAt(f++), te !== 124 && te !== 45 && te !== 58) || f >= e.eMarks[_] || (j = e.src.charCodeAt(f++), j !== 124 && j !== 45 && j !== 58 && !ui(j)) || te === 45 && ui(j)) return !1;
+        for (; f < e.eMarks[_];) {
+            if (c = e.src.charCodeAt(f), c !== 124 && c !== 45 && c !== 58 && !ui(c)) return !1;
+            f++
+        }
+        for (d = hi(e, i + 1), w = d.split("|"), L = [], g = 0; g < w.length; g++) {
+            if (R = w[g].trim(), !R) {
+                if (g === 0 || g === w.length - 1) continue;
                 return !1
             }
             if (!/^:?-+:?$/.test(R)) return !1;
             R.charCodeAt(R.length - 1) === 58 ? L.push(R.charCodeAt(0) === 58 ? "center" : "right") : R.charCodeAt(0) === 58 ? L.push("left") : L.push("")
         }
-        if (d = si(e, i).trim(), d.indexOf("|") === -1 || e.sCount[i] - e.blkIndent >= 4 || (k = Sl(d), k.length && k[0] === "" && k.shift(), k.length && k[k.length - 1] === "" && k.pop(), T = k.length, T === 0 || T !== L.length)) return !1;
+        if (d = hi(e, i).trim(), d.indexOf("|") === -1 || e.sCount[i] - e.blkIndent >= 4 || (w = Tl(d), w.length && w[0] === "" && w.shift(), w.length && w[w.length - 1] === "" && w.pop(), T = w.length, T === 0 || T !== L.length)) return !1;
         if (l) return !0;
-        for (I = e.parentType, e.parentType = "table", re = e.md.block.ruler.getRules("blockquote"), A = e.push("table_open", "table", 1), A.map = G = [i, 0], A = e.push("thead_open", "thead", 1), A.map = [i, i + 1], A = e.push("tr_open", "tr", 1), A.map = [i, i + 1], g = 0; g < k.length; g++) A = e.push("th_open", "th", 1), L[g] && (A.attrs = [
+        for (I = e.parentType, e.parentType = "table", re = e.md.block.ruler.getRules("blockquote"), A = e.push("table_open", "table", 1), A.map = O = [i, 0], A = e.push("thead_open", "thead", 1), A.map = [i, i + 1], A = e.push("tr_open", "tr", 1), A.map = [i, i + 1], g = 0; g < w.length; g++) A = e.push("th_open", "th", 1), L[g] && (A.attrs = [
             ["style", "text-align:" + L[g]]
-        ]), A = e.push("inline", "", 0), A.content = k[g].trim(), A.children = [], A = e.push("th_close", "th", -1);
+        ]), A = e.push("inline", "", 0), A.content = w[g].trim(), A.children = [], A = e.push("th_close", "th", -1);
         for (A = e.push("tr_close", "tr", -1), A = e.push("thead_close", "thead", -1), _ = i + 2; _ < a && !(e.sCount[_] < e.blkIndent); _++) {
             for (Y = !1, g = 0, y = re.length; g < y; g++)
                 if (re[g](e, _, a, !0)) {
                     Y = !0;
                     break
-                } if (Y || (d = si(e, _).trim(), !d) || e.sCount[_] - e.blkIndent >= 4) break;
-            for (k = Sl(d), k.length && k[0] === "" && k.shift(), k.length && k[k.length - 1] === "" && k.pop(), _ === i + 2 && (A = e.push("tbody_open", "tbody", 1), A.map = P = [i + 2, 0]), A = e.push("tr_open", "tr", 1), A.map = [_, _ + 1], g = 0; g < T; g++) A = e.push("td_open", "td", 1), L[g] && (A.attrs = [
+                } if (Y || (d = hi(e, _).trim(), !d) || e.sCount[_] - e.blkIndent >= 4) break;
+            for (w = Tl(d), w.length && w[0] === "" && w.shift(), w.length && w[w.length - 1] === "" && w.pop(), _ === i + 2 && (A = e.push("tbody_open", "tbody", 1), A.map = P = [i + 2, 0]), A = e.push("tr_open", "tr", 1), A.map = [_, _ + 1], g = 0; g < T; g++) A = e.push("td_open", "td", 1), L[g] && (A.attrs = [
                 ["style", "text-align:" + L[g]]
-            ]), A = e.push("inline", "", 0), A.content = k[g] ? k[g].trim() : "", A.children = [], A = e.push("td_close", "td", -1);
+            ]), A = e.push("inline", "", 0), A.content = w[g] ? w[g].trim() : "", A.children = [], A = e.push("td_close", "td", -1);
             A = e.push("tr_close", "tr", -1)
         }
-        return P && (A = e.push("tbody_close", "tbody", -1), P[1] = _), A = e.push("table_close", "table", -1), G[1] = _, e.parentType = I, e.line = _, !0
+        return P && (A = e.push("tbody_close", "tbody", -1), P[1] = _), A = e.push("table_close", "table", -1), O[1] = _, e.parentType = I, e.line = _, !0
     }
 });
-var ql = W((o2, Al) => {
+var El = W((f2, Ml) => {
     "use strict";
-    Al.exports = function(e, i, a) {
+    Ml.exports = function(e, i, a) {
         var l, c, d;
         if (e.sCount[i] - e.blkIndent < 4) return !1;
         for (c = l = i + 1; l < a;) {
             if (e.isEmpty(l)) {
                 l++;
                 continue
             }
@@ -4310,400 +4310,400 @@
             }
             break
         }
         return e.line = c, d = e.push("code_block", "code", 0), d.content = e.getLines(i, c, 4 + e.blkIndent, !1) + `
 `, d.map = [i, e.line], !0
     }
 });
-var El = W((a2, Ml) => {
+var zl = W((g2, Dl) => {
     "use strict";
-    Ml.exports = function(e, i, a, l) {
-        var c, d, m, g, y, _, k, T = !1,
+    Dl.exports = function(e, i, a, l) {
+        var c, d, f, g, y, _, w, T = !1,
             A = e.bMarks[i] + e.tShift[i],
             L = e.eMarks[i];
-        if (e.sCount[i] - e.blkIndent >= 4 || A + 3 > L || (c = e.src.charCodeAt(A), c !== 126 && c !== 96) || (y = A, A = e.skipChars(A, c), d = A - y, d < 3) || (k = e.src.slice(y, A), m = e.src.slice(A, L), c === 96 && m.indexOf(String.fromCharCode(c)) >= 0)) return !1;
+        if (e.sCount[i] - e.blkIndent >= 4 || A + 3 > L || (c = e.src.charCodeAt(A), c !== 126 && c !== 96) || (y = A, A = e.skipChars(A, c), d = A - y, d < 3) || (w = e.src.slice(y, A), f = e.src.slice(A, L), c === 96 && f.indexOf(String.fromCharCode(c)) >= 0)) return !1;
         if (l) return !0;
         for (g = i; g++, !(g >= a || (A = y = e.bMarks[g] + e.tShift[g], L = e.eMarks[g], A < L && e.sCount[g] < e.blkIndent));)
             if (e.src.charCodeAt(A) === c && !(e.sCount[g] - e.blkIndent >= 4) && (A = e.skipChars(A, c), !(A - y < d) && (A = e.skipSpaces(A), !(A < L)))) {
                 T = !0;
                 break
-            } return d = e.sCount[i], e.line = g + (T ? 1 : 0), _ = e.push("fence", "code", 0), _.info = m, _.content = e.getLines(i + 1, g, d, !0), _.markup = k, _.map = [i, e.line], !0
+            } return d = e.sCount[i], e.line = g + (T ? 1 : 0), _ = e.push("fence", "code", 0), _.info = f, _.content = e.getLines(i + 1, g, d, !0), _.markup = w, _.map = [i, e.line], !0
     }
 });
-var zl = W((s2, Dl) => {
+var Fl = W((b2, Rl) => {
     "use strict";
-    var xm = Se().isSpace;
-    Dl.exports = function(e, i, a, l) {
-        var c, d, m, g, y, _, k, T, A, L, R, G, P, I, Y, re, te, j, ne, pe, ue = e.lineMax,
+    var _m = Se().isSpace;
+    Rl.exports = function(e, i, a, l) {
+        var c, d, f, g, y, _, w, T, A, L, R, O, P, I, Y, re, te, j, ne, pe, ue = e.lineMax,
             ce = e.bMarks[i] + e.tShift[i],
             Ce = e.eMarks[i];
         if (e.sCount[i] - e.blkIndent >= 4 || e.src.charCodeAt(ce) !== 62) return !1;
         if (l) return !0;
         for (L = [], R = [], I = [], Y = [], j = e.md.block.ruler.getRules("blockquote"), P = e.parentType, e.parentType = "blockquote", T = i; T < a && (pe = e.sCount[T] < e.blkIndent, ce = e.bMarks[T] + e.tShift[T], Ce = e.eMarks[T], !(ce >= Ce)); T++) {
             if (e.src.charCodeAt(ce++) === 62 && !pe) {
-                for (g = e.sCount[T] + 1, e.src.charCodeAt(ce) === 32 ? (ce++, g++, c = !1, re = !0) : e.src.charCodeAt(ce) === 9 ? (re = !0, (e.bsCount[T] + g) % 4 === 3 ? (ce++, g++, c = !1) : c = !0) : re = !1, A = g, L.push(e.bMarks[T]), e.bMarks[T] = ce; ce < Ce && (d = e.src.charCodeAt(ce), xm(d));) {
+                for (g = e.sCount[T] + 1, e.src.charCodeAt(ce) === 32 ? (ce++, g++, c = !1, re = !0) : e.src.charCodeAt(ce) === 9 ? (re = !0, (e.bsCount[T] + g) % 4 === 3 ? (ce++, g++, c = !1) : c = !0) : re = !1, A = g, L.push(e.bMarks[T]), e.bMarks[T] = ce; ce < Ce && (d = e.src.charCodeAt(ce), _m(d));) {
                     d === 9 ? A += 4 - (A + e.bsCount[T] + (c ? 1 : 0)) % 4 : A++;
                     ce++
                 }
                 _ = ce >= Ce, R.push(e.bsCount[T]), e.bsCount[T] = e.sCount[T] + 1 + (re ? 1 : 0), I.push(e.sCount[T]), e.sCount[T] = A - g, Y.push(e.tShift[T]), e.tShift[T] = ce - e.bMarks[T];
                 continue
             }
             if (_) break;
-            for (te = !1, m = 0, y = j.length; m < y; m++)
-                if (j[m](e, T, a, !0)) {
+            for (te = !1, f = 0, y = j.length; f < y; f++)
+                if (j[f](e, T, a, !0)) {
                     te = !0;
                     break
                 } if (te) {
                 e.lineMax = T, e.blkIndent !== 0 && (L.push(e.bMarks[T]), R.push(e.bsCount[T]), Y.push(e.tShift[T]), I.push(e.sCount[T]), e.sCount[T] -= e.blkIndent);
                 break
             }
             L.push(e.bMarks[T]), R.push(e.bsCount[T]), Y.push(e.tShift[T]), I.push(e.sCount[T]), e.sCount[T] = -1
         }
-        for (G = e.blkIndent, e.blkIndent = 0, ne = e.push("blockquote_open", "blockquote", 1), ne.markup = ">", ne.map = k = [i, 0], e.md.block.tokenize(e, i, T), ne = e.push("blockquote_close", "blockquote", -1), ne.markup = ">", e.lineMax = ue, e.parentType = P, k[1] = e.line, m = 0; m < Y.length; m++) e.bMarks[m + i] = L[m], e.tShift[m + i] = Y[m], e.sCount[m + i] = I[m], e.bsCount[m + i] = R[m];
-        return e.blkIndent = G, !0
+        for (O = e.blkIndent, e.blkIndent = 0, ne = e.push("blockquote_open", "blockquote", 1), ne.markup = ">", ne.map = w = [i, 0], e.md.block.tokenize(e, i, T), ne = e.push("blockquote_close", "blockquote", -1), ne.markup = ">", e.lineMax = ue, e.parentType = P, w[1] = e.line, f = 0; f < Y.length; f++) e.bMarks[f + i] = L[f], e.tShift[f + i] = Y[f], e.sCount[f + i] = I[f], e.bsCount[f + i] = R[f];
+        return e.blkIndent = O, !0
     }
 });
-var Fl = W((l2, Rl) => {
+var Nl = W((y2, Bl) => {
     "use strict";
-    var vm = Se().isSpace;
-    Rl.exports = function(e, i, a, l) {
-        var c, d, m, g, y = e.bMarks[i] + e.tShift[i],
+    var Sm = Se().isSpace;
+    Bl.exports = function(e, i, a, l) {
+        var c, d, f, g, y = e.bMarks[i] + e.tShift[i],
             _ = e.eMarks[i];
         if (e.sCount[i] - e.blkIndent >= 4 || (c = e.src.charCodeAt(y++), c !== 42 && c !== 45 && c !== 95)) return !1;
         for (d = 1; y < _;) {
-            if (m = e.src.charCodeAt(y++), m !== c && !vm(m)) return !1;
-            m === c && d++
+            if (f = e.src.charCodeAt(y++), f !== c && !Sm(f)) return !1;
+            f === c && d++
         }
         return d < 3 ? !1 : (l || (e.line = i + 1, g = e.push("hr", "hr", 0), g.map = [i, e.line], g.markup = Array(d + 1).join(String.fromCharCode(c))), !0)
     }
 });
-var Il = W((c2, Pl) => {
+var Hl = W((x2, Ol) => {
     "use strict";
-    var Ll = Se().isSpace;
+    var Il = Se().isSpace;
 
-    function Bl(r, e) {
+    function Ll(r, e) {
         var i, a, l, c;
-        return a = r.bMarks[e] + r.tShift[e], l = r.eMarks[e], i = r.src.charCodeAt(a++), i !== 42 && i !== 45 && i !== 43 || a < l && (c = r.src.charCodeAt(a), !Ll(c)) ? -1 : a
+        return a = r.bMarks[e] + r.tShift[e], l = r.eMarks[e], i = r.src.charCodeAt(a++), i !== 42 && i !== 45 && i !== 43 || a < l && (c = r.src.charCodeAt(a), !Il(c)) ? -1 : a
     }
 
-    function Nl(r, e) {
+    function Pl(r, e) {
         var i, a = r.bMarks[e] + r.tShift[e],
             l = a,
             c = r.eMarks[e];
         if (l + 1 >= c || (i = r.src.charCodeAt(l++), i < 48 || i > 57)) return -1;
         for (;;) {
             if (l >= c) return -1;
             if (i = r.src.charCodeAt(l++), i >= 48 && i <= 57) {
                 if (l - a >= 10) return -1;
                 continue
             }
             if (i === 41 || i === 46) break;
             return -1
         }
-        return l < c && (i = r.src.charCodeAt(l), !Ll(i)) ? -1 : l
+        return l < c && (i = r.src.charCodeAt(l), !Il(i)) ? -1 : l
     }
 
-    function wm(r, e) {
+    function Cm(r, e) {
         var i, a, l = r.level + 2;
         for (i = e + 2, a = r.tokens.length - 2; i < a; i++) r.tokens[i].level === l && r.tokens[i].type === "paragraph_open" && (r.tokens[i + 2].hidden = !0, r.tokens[i].hidden = !0, i += 2)
     }
-    Pl.exports = function(e, i, a, l) {
-        var c, d, m, g, y, _, k, T, A, L, R, G, P, I, Y, re, te, j, ne, pe, ue, ce, Ce, De, U, X, he, oe = i,
+    Ol.exports = function(e, i, a, l) {
+        var c, d, f, g, y, _, w, T, A, L, R, O, P, I, Y, re, te, j, ne, pe, ue, ce, Ce, De, U, X, he, oe = i,
             ae = !1,
             ee = !0;
         if (e.sCount[oe] - e.blkIndent >= 4 || e.listIndent >= 0 && e.sCount[oe] - e.listIndent >= 4 && e.sCount[oe] < e.blkIndent) return !1;
-        if (l && e.parentType === "paragraph" && e.sCount[oe] >= e.blkIndent && (ae = !0), (ce = Nl(e, oe)) >= 0) {
-            if (k = !0, De = e.bMarks[oe] + e.tShift[oe], P = Number(e.src.slice(De, ce - 1)), ae && P !== 1) return !1
-        } else if ((ce = Bl(e, oe)) >= 0) k = !1;
+        if (l && e.parentType === "paragraph" && e.sCount[oe] >= e.blkIndent && (ae = !0), (ce = Pl(e, oe)) >= 0) {
+            if (w = !0, De = e.bMarks[oe] + e.tShift[oe], P = Number(e.src.slice(De, ce - 1)), ae && P !== 1) return !1
+        } else if ((ce = Ll(e, oe)) >= 0) w = !1;
         else return !1;
         if (ae && e.skipSpaces(ce) >= e.eMarks[oe]) return !1;
         if (l) return !0;
-        for (G = e.src.charCodeAt(ce - 1), R = e.tokens.length, k ? (he = e.push("ordered_list_open", "ol", 1), P !== 1 && (he.attrs = [
+        for (O = e.src.charCodeAt(ce - 1), R = e.tokens.length, w ? (he = e.push("ordered_list_open", "ol", 1), P !== 1 && (he.attrs = [
                 ["start", P]
-            ])) : he = e.push("bullet_list_open", "ul", 1), he.map = L = [oe, 0], he.markup = String.fromCharCode(G), Ce = !1, X = e.md.block.ruler.getRules("list"), te = e.parentType, e.parentType = "list"; oe < a;) {
+            ])) : he = e.push("bullet_list_open", "ul", 1), he.map = L = [oe, 0], he.markup = String.fromCharCode(O), Ce = !1, X = e.md.block.ruler.getRules("list"), te = e.parentType, e.parentType = "list"; oe < a;) {
             for (ue = ce, I = e.eMarks[oe], _ = Y = e.sCount[oe] + ce - (e.bMarks[oe] + e.tShift[oe]); ue < I;) {
                 if (c = e.src.charCodeAt(ue), c === 9) Y += 4 - (Y + e.bsCount[oe]) % 4;
                 else if (c === 32) Y++;
                 else break;
                 ue++
             }
-            if (d = ue, d >= I ? y = 1 : y = Y - _, y > 4 && (y = 1), g = _ + y, he = e.push("list_item_open", "li", 1), he.markup = String.fromCharCode(G), he.map = T = [oe, 0], k && (he.info = e.src.slice(De, ce - 1)), pe = e.tight, ne = e.tShift[oe], j = e.sCount[oe], re = e.listIndent, e.listIndent = e.blkIndent, e.blkIndent = g, e.tight = !0, e.tShift[oe] = d - e.bMarks[oe], e.sCount[oe] = Y, d >= I && e.isEmpty(oe + 1) ? e.line = Math.min(e.line + 2, a) : e.md.block.tokenize(e, oe, a, !0), (!e.tight || Ce) && (ee = !1), Ce = e.line - oe > 1 && e.isEmpty(e.line - 1), e.blkIndent = e.listIndent, e.listIndent = re, e.tShift[oe] = ne, e.sCount[oe] = j, e.tight = pe, he = e.push("list_item_close", "li", -1), he.markup = String.fromCharCode(G), oe = e.line, T[1] = oe, oe >= a || e.sCount[oe] < e.blkIndent || e.sCount[oe] - e.blkIndent >= 4) break;
-            for (U = !1, m = 0, A = X.length; m < A; m++)
-                if (X[m](e, oe, a, !0)) {
+            if (d = ue, d >= I ? y = 1 : y = Y - _, y > 4 && (y = 1), g = _ + y, he = e.push("list_item_open", "li", 1), he.markup = String.fromCharCode(O), he.map = T = [oe, 0], w && (he.info = e.src.slice(De, ce - 1)), pe = e.tight, ne = e.tShift[oe], j = e.sCount[oe], re = e.listIndent, e.listIndent = e.blkIndent, e.blkIndent = g, e.tight = !0, e.tShift[oe] = d - e.bMarks[oe], e.sCount[oe] = Y, d >= I && e.isEmpty(oe + 1) ? e.line = Math.min(e.line + 2, a) : e.md.block.tokenize(e, oe, a, !0), (!e.tight || Ce) && (ee = !1), Ce = e.line - oe > 1 && e.isEmpty(e.line - 1), e.blkIndent = e.listIndent, e.listIndent = re, e.tShift[oe] = ne, e.sCount[oe] = j, e.tight = pe, he = e.push("list_item_close", "li", -1), he.markup = String.fromCharCode(O), oe = e.line, T[1] = oe, oe >= a || e.sCount[oe] < e.blkIndent || e.sCount[oe] - e.blkIndent >= 4) break;
+            for (U = !1, f = 0, A = X.length; f < A; f++)
+                if (X[f](e, oe, a, !0)) {
                     U = !0;
                     break
                 } if (U) break;
-            if (k) {
-                if (ce = Nl(e, oe), ce < 0) break;
+            if (w) {
+                if (ce = Pl(e, oe), ce < 0) break;
                 De = e.bMarks[oe] + e.tShift[oe]
-            } else if (ce = Bl(e, oe), ce < 0) break;
-            if (G !== e.src.charCodeAt(ce - 1)) break
+            } else if (ce = Ll(e, oe), ce < 0) break;
+            if (O !== e.src.charCodeAt(ce - 1)) break
         }
-        return k ? he = e.push("ordered_list_close", "ol", -1) : he = e.push("bullet_list_close", "ul", -1), he.markup = String.fromCharCode(G), L[1] = oe, e.line = oe, e.parentType = te, ee && wm(e, R), !0
+        return w ? he = e.push("ordered_list_close", "ol", -1) : he = e.push("bullet_list_close", "ul", -1), he.markup = String.fromCharCode(O), L[1] = oe, e.line = oe, e.parentType = te, ee && Cm(e, R), !0
     }
 });
-var Hl = W((u2, Ol) => {
+var Gl = W((v2, $l) => {
     "use strict";
-    var km = Se().normalizeReference,
-        R0 = Se().isSpace;
-    Ol.exports = function(e, i, a, l) {
-        var c, d, m, g, y, _, k, T, A, L, R, G, P, I, Y, re, te = 0,
+    var Tm = Se().normalizeReference,
+        F0 = Se().isSpace;
+    $l.exports = function(e, i, a, l) {
+        var c, d, f, g, y, _, w, T, A, L, R, O, P, I, Y, re, te = 0,
             j = e.bMarks[i] + e.tShift[i],
             ne = e.eMarks[i],
             pe = i + 1;
         if (e.sCount[i] - e.blkIndent >= 4 || e.src.charCodeAt(j) !== 91) return !1;
         for (; ++j < ne;)
             if (e.src.charCodeAt(j) === 93 && e.src.charCodeAt(j - 1) !== 92) {
                 if (j + 1 === ne || e.src.charCodeAt(j + 1) !== 58) return !1;
                 break
             } for (g = e.lineMax, Y = e.md.block.ruler.getRules("reference"), L = e.parentType, e.parentType = "reference"; pe < g && !e.isEmpty(pe); pe++)
             if (!(e.sCount[pe] - e.blkIndent > 3) && !(e.sCount[pe] < 0)) {
-                for (I = !1, _ = 0, k = Y.length; _ < k; _++)
+                for (I = !1, _ = 0, w = Y.length; _ < w; _++)
                     if (Y[_](e, pe, g, !0)) {
                         I = !0;
                         break
                     } if (I) break
             } for (P = e.getLines(i, pe, e.blkIndent, !1).trim(), ne = P.length, j = 1; j < ne; j++) {
             if (c = P.charCodeAt(j), c === 91) return !1;
             if (c === 93) {
                 A = j;
                 break
             } else c === 10 ? te++ : c === 92 && (j++, j < ne && P.charCodeAt(j) === 10 && te++)
         }
         if (A < 0 || P.charCodeAt(A + 1) !== 58) return !1;
         for (j = A + 2; j < ne; j++)
             if (c = P.charCodeAt(j), c === 10) te++;
-            else if (!R0(c)) break;
+            else if (!F0(c)) break;
         if (R = e.md.helpers.parseLinkDestination(P, j, ne), !R.ok || (y = e.md.normalizeLink(R.str), !e.md.validateLink(y))) return !1;
-        for (j = R.pos, te += R.lines, d = j, m = te, G = j; j < ne; j++)
+        for (j = R.pos, te += R.lines, d = j, f = te, O = j; j < ne; j++)
             if (c = P.charCodeAt(j), c === 10) te++;
-            else if (!R0(c)) break;
-        for (R = e.md.helpers.parseLinkTitle(P, j, ne), j < ne && G !== j && R.ok ? (re = R.str, j = R.pos, te += R.lines) : (re = "", j = d, te = m); j < ne && (c = P.charCodeAt(j), !!R0(c));) j++;
+            else if (!F0(c)) break;
+        for (R = e.md.helpers.parseLinkTitle(P, j, ne), j < ne && O !== j && R.ok ? (re = R.str, j = R.pos, te += R.lines) : (re = "", j = d, te = f); j < ne && (c = P.charCodeAt(j), !!F0(c));) j++;
         if (j < ne && P.charCodeAt(j) !== 10 && re)
-            for (re = "", j = d, te = m; j < ne && (c = P.charCodeAt(j), !!R0(c));) j++;
-        return j < ne && P.charCodeAt(j) !== 10 || (T = km(P.slice(1, A)), !T) ? !1 : (l || (typeof e.env.references > "u" && (e.env.references = {}), typeof e.env.references[T] > "u" && (e.env.references[T] = {
+            for (re = "", j = d, te = f; j < ne && (c = P.charCodeAt(j), !!F0(c));) j++;
+        return j < ne && P.charCodeAt(j) !== 10 || (T = Tm(P.slice(1, A)), !T) ? !1 : (l || (typeof e.env.references > "u" && (e.env.references = {}), typeof e.env.references[T] > "u" && (e.env.references[T] = {
             title: re,
             href: y
         }), e.parentType = L, e.line = i + te + 1), !0)
     }
 });
-var Gl = W((h2, $l) => {
+var jl = W((w2, Vl) => {
     "use strict";
-    $l.exports = ["address", "article", "aside", "base", "basefont", "blockquote", "body", "caption", "center", "col", "colgroup", "dd", "details", "dialog", "dir", "div", "dl", "dt", "fieldset", "figcaption", "figure", "footer", "form", "frame", "frameset", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hr", "html", "iframe", "legend", "li", "link", "main", "menu", "menuitem", "nav", "noframes", "ol", "optgroup", "option", "p", "param", "section", "source", "summary", "table", "tbody", "td", "tfoot", "th", "thead", "title", "tr", "track", "ul"]
+    Vl.exports = ["address", "article", "aside", "base", "basefont", "blockquote", "body", "caption", "center", "col", "colgroup", "dd", "details", "dialog", "dir", "div", "dl", "dt", "fieldset", "figcaption", "figure", "footer", "form", "frame", "frameset", "h1", "h2", "h3", "h4", "h5", "h6", "head", "header", "hr", "html", "iframe", "legend", "li", "link", "main", "menu", "menuitem", "nav", "noframes", "ol", "optgroup", "option", "p", "param", "section", "source", "summary", "table", "tbody", "td", "tfoot", "th", "thead", "title", "tr", "track", "ul"]
 });
-var ci = W((d2, li) => {
+var mi = W((k2, di) => {
     "use strict";
-    var _m = "[a-zA-Z_:][a-zA-Z0-9:._-]*",
-        Sm = "[^\"'=<>`\\x00-\\x20]+",
-        Cm = "'[^']*'",
-        Tm = '"[^"]*"',
-        Am = "(?:" + Sm + "|" + Cm + "|" + Tm + ")",
-        qm = "(?:\\s+" + _m + "(?:\\s*=\\s*" + Am + ")?)",
-        Vl = "<[A-Za-z][A-Za-z0-9\\-]*" + qm + "*\\s*\\/?>",
-        jl = "<\\/[A-Za-z][A-Za-z0-9\\-]*\\s*>",
-        Mm = "<!---->|<!--(?:-?[^>-])(?:-?[^-])*-->",
-        Em = "<[?][\\s\\S]*?[?]>",
-        Dm = "<![A-Z]+\\s+[^>]*>",
-        zm = "<!\\[CDATA\\[[\\s\\S]*?\\]\\]>",
-        Rm = new RegExp("^(?:" + Vl + "|" + jl + "|" + Mm + "|" + Em + "|" + Dm + "|" + zm + ")"),
-        Fm = new RegExp("^(?:" + Vl + "|" + jl + ")");
-    li.exports.HTML_TAG_RE = Rm;
-    li.exports.HTML_OPEN_CLOSE_TAG_RE = Fm
+    var Am = "[a-zA-Z_:][a-zA-Z0-9:._-]*",
+        qm = "[^\"'=<>`\\x00-\\x20]+",
+        Mm = "'[^']*'",
+        Em = '"[^"]*"',
+        Dm = "(?:" + qm + "|" + Mm + "|" + Em + ")",
+        zm = "(?:\\s+" + Am + "(?:\\s*=\\s*" + Dm + ")?)",
+        Ul = "<[A-Za-z][A-Za-z0-9\\-]*" + zm + "*\\s*\\/?>",
+        Wl = "<\\/[A-Za-z][A-Za-z0-9\\-]*\\s*>",
+        Rm = "<!---->|<!--(?:-?[^>-])(?:-?[^-])*-->",
+        Fm = "<[?][\\s\\S]*?[?]>",
+        Bm = "<![A-Z]+\\s+[^>]*>",
+        Nm = "<!\\[CDATA\\[[\\s\\S]*?\\]\\]>",
+        Lm = new RegExp("^(?:" + Ul + "|" + Wl + "|" + Rm + "|" + Fm + "|" + Bm + "|" + Nm + ")"),
+        Pm = new RegExp("^(?:" + Ul + "|" + Wl + ")");
+    di.exports.HTML_TAG_RE = Lm;
+    di.exports.HTML_OPEN_CLOSE_TAG_RE = Pm
 });
-var Wl = W((m2, Ul) => {
+var Zl = W((_2, Yl) => {
     "use strict";
-    var Bm = Gl(),
-        Nm = ci().HTML_OPEN_CLOSE_TAG_RE,
+    var Im = jl(),
+        Om = mi().HTML_OPEN_CLOSE_TAG_RE,
         br = [
             [/^<(script|pre|style|textarea)(?=(\s|>|$))/i, /<\/(script|pre|style|textarea)>/i, !0],
             [/^<!--/, /-->/, !0],
             [/^<\?/, /\?>/, !0],
             [/^<![A-Z]/, />/, !0],
             [/^<!\[CDATA\[/, /\]\]>/, !0],
-            [new RegExp("^</?(" + Bm.join("|") + ")(?=(\\s|/?>|$))", "i"), /^$/, !0],
-            [new RegExp(Nm.source + "\\s*$"), /^$/, !1]
+            [new RegExp("^</?(" + Im.join("|") + ")(?=(\\s|/?>|$))", "i"), /^$/, !0],
+            [new RegExp(Om.source + "\\s*$"), /^$/, !1]
         ];
-    Ul.exports = function(e, i, a, l) {
-        var c, d, m, g, y = e.bMarks[i] + e.tShift[i],
+    Yl.exports = function(e, i, a, l) {
+        var c, d, f, g, y = e.bMarks[i] + e.tShift[i],
             _ = e.eMarks[i];
         if (e.sCount[i] - e.blkIndent >= 4 || !e.md.options.html || e.src.charCodeAt(y) !== 60) return !1;
         for (g = e.src.slice(y, _), c = 0; c < br.length && !br[c][0].test(g); c++);
         if (c === br.length) return !1;
         if (l) return br[c][2];
         if (d = i + 1, !br[c][1].test(g)) {
             for (; d < a && !(e.sCount[d] < e.blkIndent); d++)
                 if (y = e.bMarks[d] + e.tShift[d], _ = e.eMarks[d], g = e.src.slice(y, _), br[c][1].test(g)) {
                     g.length !== 0 && d++;
                     break
                 }
         }
-        return e.line = d, m = e.push("html_block", "", 0), m.map = [i, d], m.content = e.getLines(i, d, e.blkIndent, !0), !0
+        return e.line = d, f = e.push("html_block", "", 0), f.map = [i, d], f.content = e.getLines(i, d, e.blkIndent, !0), !0
     }
 });
-var Zl = W((p2, Ql) => {
+var Jl = W((S2, Xl) => {
     "use strict";
-    var Yl = Se().isSpace;
-    Ql.exports = function(e, i, a, l) {
-        var c, d, m, g, y = e.bMarks[i] + e.tShift[i],
+    var Ql = Se().isSpace;
+    Xl.exports = function(e, i, a, l) {
+        var c, d, f, g, y = e.bMarks[i] + e.tShift[i],
             _ = e.eMarks[i];
         if (e.sCount[i] - e.blkIndent >= 4 || (c = e.src.charCodeAt(y), c !== 35 || y >= _)) return !1;
         for (d = 1, c = e.src.charCodeAt(++y); c === 35 && y < _ && d <= 6;) d++, c = e.src.charCodeAt(++y);
-        return d > 6 || y < _ && !Yl(c) ? !1 : (l || (_ = e.skipSpacesBack(_, y), m = e.skipCharsBack(_, 35, y), m > y && Yl(e.src.charCodeAt(m - 1)) && (_ = m), e.line = i + 1, g = e.push("heading_open", "h" + String(d), 1), g.markup = "########".slice(0, d), g.map = [i, e.line], g = e.push("inline", "", 0), g.content = e.src.slice(y, _).trim(), g.map = [i, e.line], g.children = [], g = e.push("heading_close", "h" + String(d), -1), g.markup = "########".slice(0, d)), !0)
+        return d > 6 || y < _ && !Ql(c) ? !1 : (l || (_ = e.skipSpacesBack(_, y), f = e.skipCharsBack(_, 35, y), f > y && Ql(e.src.charCodeAt(f - 1)) && (_ = f), e.line = i + 1, g = e.push("heading_open", "h" + String(d), 1), g.markup = "########".slice(0, d), g.map = [i, e.line], g = e.push("inline", "", 0), g.content = e.src.slice(y, _).trim(), g.map = [i, e.line], g.children = [], g = e.push("heading_close", "h" + String(d), -1), g.markup = "########".slice(0, d)), !0)
     }
 });
-var Jl = W((f2, Xl) => {
+var ec = W((C2, Kl) => {
     "use strict";
-    Xl.exports = function(e, i, a) {
-        var l, c, d, m, g, y, _, k, T, A = i + 1,
+    Kl.exports = function(e, i, a) {
+        var l, c, d, f, g, y, _, w, T, A = i + 1,
             L, R = e.md.block.ruler.getRules("paragraph");
         if (e.sCount[i] - e.blkIndent >= 4) return !1;
         for (L = e.parentType, e.parentType = "paragraph"; A < a && !e.isEmpty(A); A++)
             if (!(e.sCount[A] - e.blkIndent > 3)) {
                 if (e.sCount[A] >= e.blkIndent && (y = e.bMarks[A] + e.tShift[A], _ = e.eMarks[A], y < _ && (T = e.src.charCodeAt(y), (T === 45 || T === 61) && (y = e.skipChars(y, T), y = e.skipSpaces(y), y >= _)))) {
-                    k = T === 61 ? 1 : 2;
+                    w = T === 61 ? 1 : 2;
                     break
                 }
                 if (!(e.sCount[A] < 0)) {
-                    for (c = !1, d = 0, m = R.length; d < m; d++)
+                    for (c = !1, d = 0, f = R.length; d < f; d++)
                         if (R[d](e, A, a, !0)) {
                             c = !0;
                             break
                         } if (c) break
                 }
-            } return k ? (l = e.getLines(i, A, e.blkIndent, !1).trim(), e.line = A + 1, g = e.push("heading_open", "h" + String(k), 1), g.markup = String.fromCharCode(T), g.map = [i, e.line], g = e.push("inline", "", 0), g.content = l, g.map = [i, e.line - 1], g.children = [], g = e.push("heading_close", "h" + String(k), -1), g.markup = String.fromCharCode(T), e.parentType = L, !0) : !1
+            } return w ? (l = e.getLines(i, A, e.blkIndent, !1).trim(), e.line = A + 1, g = e.push("heading_open", "h" + String(w), 1), g.markup = String.fromCharCode(T), g.map = [i, e.line], g = e.push("inline", "", 0), g.content = l, g.map = [i, e.line - 1], g.children = [], g = e.push("heading_close", "h" + String(w), -1), g.markup = String.fromCharCode(T), e.parentType = L, !0) : !1
     }
 });
-var ec = W((g2, Kl) => {
+var rc = W((T2, tc) => {
     "use strict";
-    Kl.exports = function(e, i, a) {
-        var l, c, d, m, g, y, _ = i + 1,
-            k = e.md.block.ruler.getRules("paragraph");
+    tc.exports = function(e, i, a) {
+        var l, c, d, f, g, y, _ = i + 1,
+            w = e.md.block.ruler.getRules("paragraph");
         for (y = e.parentType, e.parentType = "paragraph"; _ < a && !e.isEmpty(_); _++)
             if (!(e.sCount[_] - e.blkIndent > 3) && !(e.sCount[_] < 0)) {
-                for (c = !1, d = 0, m = k.length; d < m; d++)
-                    if (k[d](e, _, a, !0)) {
+                for (c = !1, d = 0, f = w.length; d < f; d++)
+                    if (w[d](e, _, a, !0)) {
                         c = !0;
                         break
                     } if (c) break
             } return l = e.getLines(i, _, e.blkIndent, !1).trim(), e.line = _, g = e.push("paragraph_open", "p", 1), g.map = [i, e.line], g = e.push("inline", "", 0), g.content = l, g.map = [i, e.line], g.children = [], g = e.push("paragraph_close", "p", -1), e.parentType = y, !0
     }
 });
-var nc = W((b2, rc) => {
+var oc = W((A2, ic) => {
     "use strict";
-    var tc = z0(),
-        F0 = Se().isSpace;
+    var nc = R0(),
+        B0 = Se().isSpace;
 
     function Tt(r, e, i, a) {
-        var l, c, d, m, g, y, _, k;
-        for (this.src = r, this.md = e, this.env = i, this.tokens = a, this.bMarks = [], this.eMarks = [], this.tShift = [], this.sCount = [], this.bsCount = [], this.blkIndent = 0, this.line = 0, this.lineMax = 0, this.tight = !1, this.ddIndent = -1, this.listIndent = -1, this.parentType = "root", this.level = 0, this.result = "", c = this.src, k = !1, d = m = y = _ = 0, g = c.length; m < g; m++) {
-            if (l = c.charCodeAt(m), !k)
-                if (F0(l)) {
+        var l, c, d, f, g, y, _, w;
+        for (this.src = r, this.md = e, this.env = i, this.tokens = a, this.bMarks = [], this.eMarks = [], this.tShift = [], this.sCount = [], this.bsCount = [], this.blkIndent = 0, this.line = 0, this.lineMax = 0, this.tight = !1, this.ddIndent = -1, this.listIndent = -1, this.parentType = "root", this.level = 0, this.result = "", c = this.src, w = !1, d = f = y = _ = 0, g = c.length; f < g; f++) {
+            if (l = c.charCodeAt(f), !w)
+                if (B0(l)) {
                     y++, l === 9 ? _ += 4 - _ % 4 : _++;
                     continue
-                } else k = !0;
-            (l === 10 || m === g - 1) && (l !== 10 && m++, this.bMarks.push(d), this.eMarks.push(m), this.tShift.push(y), this.sCount.push(_), this.bsCount.push(0), k = !1, y = 0, _ = 0, d = m + 1)
+                } else w = !0;
+            (l === 10 || f === g - 1) && (l !== 10 && f++, this.bMarks.push(d), this.eMarks.push(f), this.tShift.push(y), this.sCount.push(_), this.bsCount.push(0), w = !1, y = 0, _ = 0, d = f + 1)
         }
         this.bMarks.push(c.length), this.eMarks.push(c.length), this.tShift.push(0), this.sCount.push(0), this.bsCount.push(0), this.lineMax = this.bMarks.length - 1
     }
     Tt.prototype.push = function(r, e, i) {
-        var a = new tc(r, e, i);
+        var a = new nc(r, e, i);
         return a.block = !0, i < 0 && this.level--, a.level = this.level, i > 0 && this.level++, this.tokens.push(a), a
     };
     Tt.prototype.isEmpty = function(e) {
         return this.bMarks[e] + this.tShift[e] >= this.eMarks[e]
     };
     Tt.prototype.skipEmptyLines = function(e) {
         for (var i = this.lineMax; e < i && !(this.bMarks[e] + this.tShift[e] < this.eMarks[e]); e++);
         return e
     };
     Tt.prototype.skipSpaces = function(e) {
-        for (var i, a = this.src.length; e < a && (i = this.src.charCodeAt(e), !!F0(i)); e++);
+        for (var i, a = this.src.length; e < a && (i = this.src.charCodeAt(e), !!B0(i)); e++);
         return e
     };
     Tt.prototype.skipSpacesBack = function(e, i) {
         if (e <= i) return e;
         for (; e > i;)
-            if (!F0(this.src.charCodeAt(--e))) return e + 1;
+            if (!B0(this.src.charCodeAt(--e))) return e + 1;
         return e
     };
     Tt.prototype.skipChars = function(e, i) {
         for (var a = this.src.length; e < a && this.src.charCodeAt(e) === i; e++);
         return e
     };
     Tt.prototype.skipCharsBack = function(e, i, a) {
         if (e <= a) return e;
         for (; e > a;)
             if (i !== this.src.charCodeAt(--e)) return e + 1;
         return e
     };
     Tt.prototype.getLines = function(e, i, a, l) {
-        var c, d, m, g, y, _, k, T = e;
+        var c, d, f, g, y, _, w, T = e;
         if (e >= i) return "";
         for (_ = new Array(i - e), c = 0; T < i; T++, c++) {
-            for (d = 0, k = g = this.bMarks[T], T + 1 < i || l ? y = this.eMarks[T] + 1 : y = this.eMarks[T]; g < y && d < a;) {
-                if (m = this.src.charCodeAt(g), F0(m)) m === 9 ? d += 4 - (d + this.bsCount[T]) % 4 : d++;
-                else if (g - k < this.tShift[T]) d++;
+            for (d = 0, w = g = this.bMarks[T], T + 1 < i || l ? y = this.eMarks[T] + 1 : y = this.eMarks[T]; g < y && d < a;) {
+                if (f = this.src.charCodeAt(g), B0(f)) f === 9 ? d += 4 - (d + this.bsCount[T]) % 4 : d++;
+                else if (g - w < this.tShift[T]) d++;
                 else break;
                 g++
             }
             d > a ? _[c] = new Array(d - a + 1).join(" ") + this.src.slice(g, y) : _[c] = this.src.slice(g, y)
         }
         return _.join("")
     };
-    Tt.prototype.Token = tc;
-    rc.exports = Tt
+    Tt.prototype.Token = nc;
+    ic.exports = Tt
 });
-var oc = W((y2, ic) => {
+var sc = W((q2, ac) => {
     "use strict";
-    var Lm = E0(),
-        B0 = [
-            ["table", Tl(), ["paragraph", "reference"]],
-            ["code", ql()],
-            ["fence", El(), ["paragraph", "reference", "blockquote", "list"]],
-            ["blockquote", zl(), ["paragraph", "reference", "blockquote", "list"]],
-            ["hr", Fl(), ["paragraph", "reference", "blockquote", "list"]],
-            ["list", Il(), ["paragraph", "reference", "blockquote"]],
-            ["reference", Hl()],
-            ["html_block", Wl(), ["paragraph", "reference", "blockquote"]],
-            ["heading", Zl(), ["paragraph", "reference", "blockquote"]],
-            ["lheading", Jl()],
-            ["paragraph", ec()]
+    var Hm = D0(),
+        N0 = [
+            ["table", ql(), ["paragraph", "reference"]],
+            ["code", El()],
+            ["fence", zl(), ["paragraph", "reference", "blockquote", "list"]],
+            ["blockquote", Fl(), ["paragraph", "reference", "blockquote", "list"]],
+            ["hr", Nl(), ["paragraph", "reference", "blockquote", "list"]],
+            ["list", Hl(), ["paragraph", "reference", "blockquote"]],
+            ["reference", Gl()],
+            ["html_block", Zl(), ["paragraph", "reference", "blockquote"]],
+            ["heading", Jl(), ["paragraph", "reference", "blockquote"]],
+            ["lheading", ec()],
+            ["paragraph", rc()]
         ];
 
-    function N0() {
-        this.ruler = new Lm;
-        for (var r = 0; r < B0.length; r++) this.ruler.push(B0[r][0], B0[r][1], {
-            alt: (B0[r][2] || []).slice()
+    function L0() {
+        this.ruler = new Hm;
+        for (var r = 0; r < N0.length; r++) this.ruler.push(N0[r][0], N0[r][1], {
+            alt: (N0[r][2] || []).slice()
         })
     }
-    N0.prototype.tokenize = function(r, e, i) {
-        for (var a, l, c, d = this.ruler.getRules(""), m = d.length, g = e, y = !1, _ = r.md.options.maxNesting; g < i && (r.line = g = r.skipEmptyLines(g), !(g >= i || r.sCount[g] < r.blkIndent));) {
+    L0.prototype.tokenize = function(r, e, i) {
+        for (var a, l, c, d = this.ruler.getRules(""), f = d.length, g = e, y = !1, _ = r.md.options.maxNesting; g < i && (r.line = g = r.skipEmptyLines(g), !(g >= i || r.sCount[g] < r.blkIndent));) {
             if (r.level >= _) {
                 r.line = i;
                 break
             }
-            for (c = r.line, l = 0; l < m; l++)
+            for (c = r.line, l = 0; l < f; l++)
                 if (a = d[l](r, g, i, !1), a) {
                     if (c >= r.line) throw new Error("block rule didn't increment state.line");
                     break
                 } if (!a) throw new Error("none of the block rules matched");
             r.tight = !y, r.isEmpty(r.line - 1) && (y = !0), g = r.line, g < i && r.isEmpty(g) && (y = !0, g++, r.line = g)
         }
     };
-    N0.prototype.parse = function(r, e, i, a) {
+    L0.prototype.parse = function(r, e, i, a) {
         var l;
         r && (l = new this.State(r, e, i, a), this.tokenize(l, l.line, l.lineMax))
     };
-    N0.prototype.State = nc();
-    ic.exports = N0
+    L0.prototype.State = oc();
+    ac.exports = L0
 });
-var sc = W((x2, ac) => {
+var cc = W((M2, lc) => {
     "use strict";
 
-    function Pm(r) {
+    function $m(r) {
         switch (r) {
             case 10:
             case 33:
             case 35:
             case 36:
             case 37:
             case 38:
@@ -4725,384 +4725,384 @@
             case 125:
             case 126:
                 return !0;
             default:
                 return !1
         }
     }
-    ac.exports = function(e, i) {
-        for (var a = e.pos; a < e.posMax && !Pm(e.src.charCodeAt(a));) a++;
+    lc.exports = function(e, i) {
+        for (var a = e.pos; a < e.posMax && !$m(e.src.charCodeAt(a));) a++;
         return a === e.pos ? !1 : (i || (e.pending += e.src.slice(e.pos, a)), e.pos = a, !0)
     }
 });
-var cc = W((v2, lc) => {
+var hc = W((E2, uc) => {
     "use strict";
-    var Im = /(?:^|[^a-z0-9.+-])([a-z][a-z0-9.+-]*)$/i;
-    lc.exports = function(e, i) {
-        var a, l, c, d, m, g, y, _;
-        return !e.md.options.linkify || e.linkLevel > 0 || (a = e.pos, l = e.posMax, a + 3 > l) || e.src.charCodeAt(a) !== 58 || e.src.charCodeAt(a + 1) !== 47 || e.src.charCodeAt(a + 2) !== 47 || (c = e.pending.match(Im), !c) || (d = c[1], m = e.md.linkify.matchAtStart(e.src.slice(a - d.length)), !m) || (g = m.url, g.length <= d.length) || (g = g.replace(/\*+$/, ""), y = e.md.normalizeLink(g), !e.md.validateLink(y)) ? !1 : (i || (e.pending = e.pending.slice(0, -d.length), _ = e.push("link_open", "a", 1), _.attrs = [
+    var Gm = /(?:^|[^a-z0-9.+-])([a-z][a-z0-9.+-]*)$/i;
+    uc.exports = function(e, i) {
+        var a, l, c, d, f, g, y, _;
+        return !e.md.options.linkify || e.linkLevel > 0 || (a = e.pos, l = e.posMax, a + 3 > l) || e.src.charCodeAt(a) !== 58 || e.src.charCodeAt(a + 1) !== 47 || e.src.charCodeAt(a + 2) !== 47 || (c = e.pending.match(Gm), !c) || (d = c[1], f = e.md.linkify.matchAtStart(e.src.slice(a - d.length)), !f) || (g = f.url, g.length <= d.length) || (g = g.replace(/\*+$/, ""), y = e.md.normalizeLink(g), !e.md.validateLink(y)) ? !1 : (i || (e.pending = e.pending.slice(0, -d.length), _ = e.push("link_open", "a", 1), _.attrs = [
             ["href", y]
         ], _.markup = "linkify", _.info = "auto", _ = e.push("text", "", 0), _.content = e.md.normalizeLinkText(g), _ = e.push("link_close", "a", -1), _.markup = "linkify", _.info = "auto"), e.pos += g.length - d.length, !0)
     }
 });
-var hc = W((w2, uc) => {
+var mc = W((D2, dc) => {
     "use strict";
-    var Om = Se().isSpace;
-    uc.exports = function(e, i) {
+    var Vm = Se().isSpace;
+    dc.exports = function(e, i) {
         var a, l, c, d = e.pos;
         if (e.src.charCodeAt(d) !== 10) return !1;
         if (a = e.pending.length - 1, l = e.posMax, !i)
             if (a >= 0 && e.pending.charCodeAt(a) === 32)
                 if (a >= 1 && e.pending.charCodeAt(a - 1) === 32) {
                     for (c = a - 1; c >= 1 && e.pending.charCodeAt(c - 1) === 32;) c--;
                     e.pending = e.pending.slice(0, c), e.push("hardbreak", "br", 0)
                 } else e.pending = e.pending.slice(0, -1), e.push("softbreak", "br", 0);
         else e.push("softbreak", "br", 0);
-        for (d++; d < l && Om(e.src.charCodeAt(d));) d++;
+        for (d++; d < l && Vm(e.src.charCodeAt(d));) d++;
         return e.pos = d, !0
     }
 });
-var mc = W((k2, dc) => {
+var fc = W((z2, pc) => {
     "use strict";
-    var Hm = Se().isSpace,
-        hi = [];
-    for (ui = 0; ui < 256; ui++) hi.push(0);
-    var ui;
+    var jm = Se().isSpace,
+        fi = [];
+    for (pi = 0; pi < 256; pi++) fi.push(0);
+    var pi;
     "\\!\"#$%&'()*+,./:;<=>?@[]^_`{|}~-".split("").forEach(function(r) {
-        hi[r.charCodeAt(0)] = 1
+        fi[r.charCodeAt(0)] = 1
     });
-    dc.exports = function(e, i) {
-        var a, l, c, d, m, g = e.pos,
+    pc.exports = function(e, i) {
+        var a, l, c, d, f, g = e.pos,
             y = e.posMax;
         if (e.src.charCodeAt(g) !== 92 || (g++, g >= y)) return !1;
         if (a = e.src.charCodeAt(g), a === 10) {
-            for (i || e.push("hardbreak", "br", 0), g++; g < y && (a = e.src.charCodeAt(g), !!Hm(a));) g++;
+            for (i || e.push("hardbreak", "br", 0), g++; g < y && (a = e.src.charCodeAt(g), !!jm(a));) g++;
             return e.pos = g, !0
         }
-        return d = e.src[g], a >= 55296 && a <= 56319 && g + 1 < y && (l = e.src.charCodeAt(g + 1), l >= 56320 && l <= 57343 && (d += e.src[g + 1], g++)), c = "\\" + d, i || (m = e.push("text_special", "", 0), a < 256 && hi[a] !== 0 ? m.content = d : m.content = c, m.markup = c, m.info = "escape"), e.pos = g + 1, !0
+        return d = e.src[g], a >= 55296 && a <= 56319 && g + 1 < y && (l = e.src.charCodeAt(g + 1), l >= 56320 && l <= 57343 && (d += e.src[g + 1], g++)), c = "\\" + d, i || (f = e.push("text_special", "", 0), a < 256 && fi[a] !== 0 ? f.content = d : f.content = c, f.markup = c, f.info = "escape"), e.pos = g + 1, !0
     }
 });
-var fc = W((_2, pc) => {
+var bc = W((R2, gc) => {
     "use strict";
-    pc.exports = function(e, i) {
-        var a, l, c, d, m, g, y, _, k = e.pos,
-            T = e.src.charCodeAt(k);
+    gc.exports = function(e, i) {
+        var a, l, c, d, f, g, y, _, w = e.pos,
+            T = e.src.charCodeAt(w);
         if (T !== 96) return !1;
-        for (a = k, k++, l = e.posMax; k < l && e.src.charCodeAt(k) === 96;) k++;
-        if (c = e.src.slice(a, k), y = c.length, e.backticksScanned && (e.backticks[y] || 0) <= a) return i || (e.pending += c), e.pos += y, !0;
-        for (g = k;
-            (m = e.src.indexOf("`", g)) !== -1;) {
-            for (g = m + 1; g < l && e.src.charCodeAt(g) === 96;) g++;
-            if (_ = g - m, _ === y) return i || (d = e.push("code_inline", "code", 0), d.markup = c, d.content = e.src.slice(k, m).replace(/\n/g, " ").replace(/^ (.+) $/, "$1")), e.pos = g, !0;
-            e.backticks[_] = m
+        for (a = w, w++, l = e.posMax; w < l && e.src.charCodeAt(w) === 96;) w++;
+        if (c = e.src.slice(a, w), y = c.length, e.backticksScanned && (e.backticks[y] || 0) <= a) return i || (e.pending += c), e.pos += y, !0;
+        for (g = w;
+            (f = e.src.indexOf("`", g)) !== -1;) {
+            for (g = f + 1; g < l && e.src.charCodeAt(g) === 96;) g++;
+            if (_ = g - f, _ === y) return i || (d = e.push("code_inline", "code", 0), d.markup = c, d.content = e.src.slice(w, f).replace(/\n/g, " ").replace(/^ (.+) $/, "$1")), e.pos = g, !0;
+            e.backticks[_] = f
         }
         return e.backticksScanned = !0, i || (e.pending += c), e.pos += y, !0
     }
 });
-var mi = W((S2, di) => {
+var bi = W((F2, gi) => {
     "use strict";
-    di.exports.tokenize = function(e, i) {
-        var a, l, c, d, m, g = e.pos,
+    gi.exports.tokenize = function(e, i) {
+        var a, l, c, d, f, g = e.pos,
             y = e.src.charCodeAt(g);
-        if (i || y !== 126 || (l = e.scanDelims(e.pos, !0), d = l.length, m = String.fromCharCode(y), d < 2)) return !1;
-        for (d % 2 && (c = e.push("text", "", 0), c.content = m, d--), a = 0; a < d; a += 2) c = e.push("text", "", 0), c.content = m + m, e.delimiters.push({
+        if (i || y !== 126 || (l = e.scanDelims(e.pos, !0), d = l.length, f = String.fromCharCode(y), d < 2)) return !1;
+        for (d % 2 && (c = e.push("text", "", 0), c.content = f, d--), a = 0; a < d; a += 2) c = e.push("text", "", 0), c.content = f + f, e.delimiters.push({
             marker: y,
             length: 0,
             token: e.tokens.length - 1,
             end: -1,
             open: l.can_open,
             close: l.can_close
         });
         return e.pos += l.length, !0
     };
 
-    function gc(r, e) {
-        var i, a, l, c, d, m = [],
+    function yc(r, e) {
+        var i, a, l, c, d, f = [],
             g = e.length;
-        for (i = 0; i < g; i++) l = e[i], l.marker === 126 && l.end !== -1 && (c = e[l.end], d = r.tokens[l.token], d.type = "s_open", d.tag = "s", d.nesting = 1, d.markup = "~~", d.content = "", d = r.tokens[c.token], d.type = "s_close", d.tag = "s", d.nesting = -1, d.markup = "~~", d.content = "", r.tokens[c.token - 1].type === "text" && r.tokens[c.token - 1].content === "~" && m.push(c.token - 1));
-        for (; m.length;) {
-            for (i = m.pop(), a = i + 1; a < r.tokens.length && r.tokens[a].type === "s_close";) a++;
+        for (i = 0; i < g; i++) l = e[i], l.marker === 126 && l.end !== -1 && (c = e[l.end], d = r.tokens[l.token], d.type = "s_open", d.tag = "s", d.nesting = 1, d.markup = "~~", d.content = "", d = r.tokens[c.token], d.type = "s_close", d.tag = "s", d.nesting = -1, d.markup = "~~", d.content = "", r.tokens[c.token - 1].type === "text" && r.tokens[c.token - 1].content === "~" && f.push(c.token - 1));
+        for (; f.length;) {
+            for (i = f.pop(), a = i + 1; a < r.tokens.length && r.tokens[a].type === "s_close";) a++;
             a--, i !== a && (d = r.tokens[a], r.tokens[a] = r.tokens[i], r.tokens[i] = d)
         }
     }
-    di.exports.postProcess = function(e) {
+    gi.exports.postProcess = function(e) {
         var i, a = e.tokens_meta,
             l = e.tokens_meta.length;
-        for (gc(e, e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && gc(e, a[i].delimiters)
+        for (yc(e, e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && yc(e, a[i].delimiters)
     }
 });
-var fi = W((C2, pi) => {
+var xi = W((B2, yi) => {
     "use strict";
-    pi.exports.tokenize = function(e, i) {
+    yi.exports.tokenize = function(e, i) {
         var a, l, c, d = e.pos,
-            m = e.src.charCodeAt(d);
-        if (i || m !== 95 && m !== 42) return !1;
-        for (l = e.scanDelims(e.pos, m === 42), a = 0; a < l.length; a++) c = e.push("text", "", 0), c.content = String.fromCharCode(m), e.delimiters.push({
-            marker: m,
+            f = e.src.charCodeAt(d);
+        if (i || f !== 95 && f !== 42) return !1;
+        for (l = e.scanDelims(e.pos, f === 42), a = 0; a < l.length; a++) c = e.push("text", "", 0), c.content = String.fromCharCode(f), e.delimiters.push({
+            marker: f,
             length: l.length,
             token: e.tokens.length - 1,
             end: -1,
             open: l.can_open,
             close: l.can_close
         });
         return e.pos += l.length, !0
     };
 
-    function bc(r, e) {
-        var i, a, l, c, d, m, g = e.length;
-        for (i = g - 1; i >= 0; i--) a = e[i], !(a.marker !== 95 && a.marker !== 42) && a.end !== -1 && (l = e[a.end], m = i > 0 && e[i - 1].end === a.end + 1 && e[i - 1].marker === a.marker && e[i - 1].token === a.token - 1 && e[a.end + 1].token === l.token + 1, d = String.fromCharCode(a.marker), c = r.tokens[a.token], c.type = m ? "strong_open" : "em_open", c.tag = m ? "strong" : "em", c.nesting = 1, c.markup = m ? d + d : d, c.content = "", c = r.tokens[l.token], c.type = m ? "strong_close" : "em_close", c.tag = m ? "strong" : "em", c.nesting = -1, c.markup = m ? d + d : d, c.content = "", m && (r.tokens[e[i - 1].token].content = "", r.tokens[e[a.end + 1].token].content = "", i--))
+    function xc(r, e) {
+        var i, a, l, c, d, f, g = e.length;
+        for (i = g - 1; i >= 0; i--) a = e[i], !(a.marker !== 95 && a.marker !== 42) && a.end !== -1 && (l = e[a.end], f = i > 0 && e[i - 1].end === a.end + 1 && e[i - 1].marker === a.marker && e[i - 1].token === a.token - 1 && e[a.end + 1].token === l.token + 1, d = String.fromCharCode(a.marker), c = r.tokens[a.token], c.type = f ? "strong_open" : "em_open", c.tag = f ? "strong" : "em", c.nesting = 1, c.markup = f ? d + d : d, c.content = "", c = r.tokens[l.token], c.type = f ? "strong_close" : "em_close", c.tag = f ? "strong" : "em", c.nesting = -1, c.markup = f ? d + d : d, c.content = "", f && (r.tokens[e[i - 1].token].content = "", r.tokens[e[a.end + 1].token].content = "", i--))
     }
-    pi.exports.postProcess = function(e) {
+    yi.exports.postProcess = function(e) {
         var i, a = e.tokens_meta,
             l = e.tokens_meta.length;
-        for (bc(e, e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && bc(e, a[i].delimiters)
+        for (xc(e, e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && xc(e, a[i].delimiters)
     }
 });
-var xc = W((T2, yc) => {
+var wc = W((N2, vc) => {
     "use strict";
-    var $m = Se().normalizeReference,
-        gi = Se().isSpace;
-    yc.exports = function(e, i) {
-        var a, l, c, d, m, g, y, _, k, T = "",
+    var Um = Se().normalizeReference,
+        vi = Se().isSpace;
+    vc.exports = function(e, i) {
+        var a, l, c, d, f, g, y, _, w, T = "",
             A = "",
             L = e.pos,
             R = e.posMax,
-            G = e.pos,
+            O = e.pos,
             P = !0;
-        if (e.src.charCodeAt(e.pos) !== 91 || (m = e.pos + 1, d = e.md.helpers.parseLinkLabel(e, e.pos, !0), d < 0)) return !1;
+        if (e.src.charCodeAt(e.pos) !== 91 || (f = e.pos + 1, d = e.md.helpers.parseLinkLabel(e, e.pos, !0), d < 0)) return !1;
         if (g = d + 1, g < R && e.src.charCodeAt(g) === 40) {
-            for (P = !1, g++; g < R && (l = e.src.charCodeAt(g), !(!gi(l) && l !== 10)); g++);
+            for (P = !1, g++; g < R && (l = e.src.charCodeAt(g), !(!vi(l) && l !== 10)); g++);
             if (g >= R) return !1;
-            if (G = g, y = e.md.helpers.parseLinkDestination(e.src, g, e.posMax), y.ok) {
-                for (T = e.md.normalizeLink(y.str), e.md.validateLink(T) ? g = y.pos : T = "", G = g; g < R && (l = e.src.charCodeAt(g), !(!gi(l) && l !== 10)); g++);
-                if (y = e.md.helpers.parseLinkTitle(e.src, g, e.posMax), g < R && G !== g && y.ok)
-                    for (A = y.str, g = y.pos; g < R && (l = e.src.charCodeAt(g), !(!gi(l) && l !== 10)); g++);
+            if (O = g, y = e.md.helpers.parseLinkDestination(e.src, g, e.posMax), y.ok) {
+                for (T = e.md.normalizeLink(y.str), e.md.validateLink(T) ? g = y.pos : T = "", O = g; g < R && (l = e.src.charCodeAt(g), !(!vi(l) && l !== 10)); g++);
+                if (y = e.md.helpers.parseLinkTitle(e.src, g, e.posMax), g < R && O !== g && y.ok)
+                    for (A = y.str, g = y.pos; g < R && (l = e.src.charCodeAt(g), !(!vi(l) && l !== 10)); g++);
             }(g >= R || e.src.charCodeAt(g) !== 41) && (P = !0), g++
         }
         if (P) {
             if (typeof e.env.references > "u") return !1;
-            if (g < R && e.src.charCodeAt(g) === 91 ? (G = g + 1, g = e.md.helpers.parseLinkLabel(e, g), g >= 0 ? c = e.src.slice(G, g++) : g = d + 1) : g = d + 1, c || (c = e.src.slice(m, d)), _ = e.env.references[$m(c)], !_) return e.pos = L, !1;
+            if (g < R && e.src.charCodeAt(g) === 91 ? (O = g + 1, g = e.md.helpers.parseLinkLabel(e, g), g >= 0 ? c = e.src.slice(O, g++) : g = d + 1) : g = d + 1, c || (c = e.src.slice(f, d)), _ = e.env.references[Um(c)], !_) return e.pos = L, !1;
             T = _.href, A = _.title
         }
-        return i || (e.pos = m, e.posMax = d, k = e.push("link_open", "a", 1), k.attrs = a = [
+        return i || (e.pos = f, e.posMax = d, w = e.push("link_open", "a", 1), w.attrs = a = [
             ["href", T]
-        ], A && a.push(["title", A]), e.linkLevel++, e.md.inline.tokenize(e), e.linkLevel--, k = e.push("link_close", "a", -1)), e.pos = g, e.posMax = R, !0
+        ], A && a.push(["title", A]), e.linkLevel++, e.md.inline.tokenize(e), e.linkLevel--, w = e.push("link_close", "a", -1)), e.pos = g, e.posMax = R, !0
     }
 });
-var wc = W((A2, vc) => {
+var _c = W((L2, kc) => {
     "use strict";
-    var Gm = Se().normalizeReference,
-        bi = Se().isSpace;
-    vc.exports = function(e, i) {
-        var a, l, c, d, m, g, y, _, k, T, A, L, R, G = "",
+    var Wm = Se().normalizeReference,
+        wi = Se().isSpace;
+    kc.exports = function(e, i) {
+        var a, l, c, d, f, g, y, _, w, T, A, L, R, O = "",
             P = e.pos,
             I = e.posMax;
-        if (e.src.charCodeAt(e.pos) !== 33 || e.src.charCodeAt(e.pos + 1) !== 91 || (g = e.pos + 2, m = e.md.helpers.parseLinkLabel(e, e.pos + 1, !1), m < 0)) return !1;
-        if (y = m + 1, y < I && e.src.charCodeAt(y) === 40) {
-            for (y++; y < I && (l = e.src.charCodeAt(y), !(!bi(l) && l !== 10)); y++);
+        if (e.src.charCodeAt(e.pos) !== 33 || e.src.charCodeAt(e.pos + 1) !== 91 || (g = e.pos + 2, f = e.md.helpers.parseLinkLabel(e, e.pos + 1, !1), f < 0)) return !1;
+        if (y = f + 1, y < I && e.src.charCodeAt(y) === 40) {
+            for (y++; y < I && (l = e.src.charCodeAt(y), !(!wi(l) && l !== 10)); y++);
             if (y >= I) return !1;
-            for (R = y, k = e.md.helpers.parseLinkDestination(e.src, y, e.posMax), k.ok && (G = e.md.normalizeLink(k.str), e.md.validateLink(G) ? y = k.pos : G = ""), R = y; y < I && (l = e.src.charCodeAt(y), !(!bi(l) && l !== 10)); y++);
-            if (k = e.md.helpers.parseLinkTitle(e.src, y, e.posMax), y < I && R !== y && k.ok)
-                for (T = k.str, y = k.pos; y < I && (l = e.src.charCodeAt(y), !(!bi(l) && l !== 10)); y++);
+            for (R = y, w = e.md.helpers.parseLinkDestination(e.src, y, e.posMax), w.ok && (O = e.md.normalizeLink(w.str), e.md.validateLink(O) ? y = w.pos : O = ""), R = y; y < I && (l = e.src.charCodeAt(y), !(!wi(l) && l !== 10)); y++);
+            if (w = e.md.helpers.parseLinkTitle(e.src, y, e.posMax), y < I && R !== y && w.ok)
+                for (T = w.str, y = w.pos; y < I && (l = e.src.charCodeAt(y), !(!wi(l) && l !== 10)); y++);
             else T = "";
             if (y >= I || e.src.charCodeAt(y) !== 41) return e.pos = P, !1;
             y++
         } else {
             if (typeof e.env.references > "u") return !1;
-            if (y < I && e.src.charCodeAt(y) === 91 ? (R = y + 1, y = e.md.helpers.parseLinkLabel(e, y), y >= 0 ? d = e.src.slice(R, y++) : y = m + 1) : y = m + 1, d || (d = e.src.slice(g, m)), _ = e.env.references[Gm(d)], !_) return e.pos = P, !1;
-            G = _.href, T = _.title
+            if (y < I && e.src.charCodeAt(y) === 91 ? (R = y + 1, y = e.md.helpers.parseLinkLabel(e, y), y >= 0 ? d = e.src.slice(R, y++) : y = f + 1) : y = f + 1, d || (d = e.src.slice(g, f)), _ = e.env.references[Wm(d)], !_) return e.pos = P, !1;
+            O = _.href, T = _.title
         }
-        return i || (c = e.src.slice(g, m), e.md.inline.parse(c, e.md, e.env, L = []), A = e.push("image", "img", 0), A.attrs = a = [
-            ["src", G],
+        return i || (c = e.src.slice(g, f), e.md.inline.parse(c, e.md, e.env, L = []), A = e.push("image", "img", 0), A.attrs = a = [
+            ["src", O],
             ["alt", ""]
         ], A.children = L, A.content = c, T && a.push(["title", T])), e.pos = y, e.posMax = I, !0
     }
 });
-var _c = W((q2, kc) => {
+var Cc = W((P2, Sc) => {
     "use strict";
-    var Vm = /^([a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*)$/,
-        jm = /^([a-zA-Z][a-zA-Z0-9+.\-]{1,31}):([^<>\x00-\x20]*)$/;
-    kc.exports = function(e, i) {
-        var a, l, c, d, m, g, y = e.pos;
+    var Ym = /^([a-zA-Z0-9.!#$%&'*+\/=?^_`{|}~-]+@[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?(?:\.[a-zA-Z0-9](?:[a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?)*)$/,
+        Zm = /^([a-zA-Z][a-zA-Z0-9+.\-]{1,31}):([^<>\x00-\x20]*)$/;
+    Sc.exports = function(e, i) {
+        var a, l, c, d, f, g, y = e.pos;
         if (e.src.charCodeAt(y) !== 60) return !1;
-        for (m = e.pos, g = e.posMax;;) {
+        for (f = e.pos, g = e.posMax;;) {
             if (++y >= g || (d = e.src.charCodeAt(y), d === 60)) return !1;
             if (d === 62) break
         }
-        return a = e.src.slice(m + 1, y), jm.test(a) ? (l = e.md.normalizeLink(a), e.md.validateLink(l) ? (i || (c = e.push("link_open", "a", 1), c.attrs = [
+        return a = e.src.slice(f + 1, y), Zm.test(a) ? (l = e.md.normalizeLink(a), e.md.validateLink(l) ? (i || (c = e.push("link_open", "a", 1), c.attrs = [
             ["href", l]
-        ], c.markup = "autolink", c.info = "auto", c = e.push("text", "", 0), c.content = e.md.normalizeLinkText(a), c = e.push("link_close", "a", -1), c.markup = "autolink", c.info = "auto"), e.pos += a.length + 2, !0) : !1) : Vm.test(a) ? (l = e.md.normalizeLink("mailto:" + a), e.md.validateLink(l) ? (i || (c = e.push("link_open", "a", 1), c.attrs = [
+        ], c.markup = "autolink", c.info = "auto", c = e.push("text", "", 0), c.content = e.md.normalizeLinkText(a), c = e.push("link_close", "a", -1), c.markup = "autolink", c.info = "auto"), e.pos += a.length + 2, !0) : !1) : Ym.test(a) ? (l = e.md.normalizeLink("mailto:" + a), e.md.validateLink(l) ? (i || (c = e.push("link_open", "a", 1), c.attrs = [
             ["href", l]
         ], c.markup = "autolink", c.info = "auto", c = e.push("text", "", 0), c.content = e.md.normalizeLinkText(a), c = e.push("link_close", "a", -1), c.markup = "autolink", c.info = "auto"), e.pos += a.length + 2, !0) : !1) : !1
     }
 });
-var Cc = W((M2, Sc) => {
+var Ac = W((I2, Tc) => {
     "use strict";
-    var Um = ci().HTML_TAG_RE;
+    var Qm = mi().HTML_TAG_RE;
 
-    function Wm(r) {
+    function Xm(r) {
         return /^<a[>\s]/i.test(r)
     }
 
-    function Ym(r) {
+    function Jm(r) {
         return /^<\/a\s*>/i.test(r)
     }
 
-    function Qm(r) {
+    function Km(r) {
         var e = r | 32;
         return e >= 97 && e <= 122
     }
-    Sc.exports = function(e, i) {
-        var a, l, c, d, m = e.pos;
-        return !e.md.options.html || (c = e.posMax, e.src.charCodeAt(m) !== 60 || m + 2 >= c) || (a = e.src.charCodeAt(m + 1), a !== 33 && a !== 63 && a !== 47 && !Qm(a)) || (l = e.src.slice(m).match(Um), !l) ? !1 : (i || (d = e.push("html_inline", "", 0), d.content = l[0], Wm(d.content) && e.linkLevel++, Ym(d.content) && e.linkLevel--), e.pos += l[0].length, !0)
+    Tc.exports = function(e, i) {
+        var a, l, c, d, f = e.pos;
+        return !e.md.options.html || (c = e.posMax, e.src.charCodeAt(f) !== 60 || f + 2 >= c) || (a = e.src.charCodeAt(f + 1), a !== 33 && a !== 63 && a !== 47 && !Km(a)) || (l = e.src.slice(f).match(Qm), !l) ? !1 : (i || (d = e.push("html_inline", "", 0), d.content = l[0], Xm(d.content) && e.linkLevel++, Jm(d.content) && e.linkLevel--), e.pos += l[0].length, !0)
     }
 });
-var Mc = W((E2, qc) => {
+var Dc = W((O2, Ec) => {
     "use strict";
-    var Tc = Kn(),
-        Zm = Se().has,
-        Xm = Se().isValidEntityCode,
-        Ac = Se().fromCodePoint,
-        Jm = /^&#((?:x[a-f0-9]{1,6}|[0-9]{1,7}));/i,
-        Km = /^&([a-z][a-z0-9]{1,31});/i;
-    qc.exports = function(e, i) {
-        var a, l, c, d, m = e.pos,
+    var qc = ni(),
+        ep = Se().has,
+        tp = Se().isValidEntityCode,
+        Mc = Se().fromCodePoint,
+        rp = /^&#((?:x[a-f0-9]{1,6}|[0-9]{1,7}));/i,
+        np = /^&([a-z][a-z0-9]{1,31});/i;
+    Ec.exports = function(e, i) {
+        var a, l, c, d, f = e.pos,
             g = e.posMax;
-        if (e.src.charCodeAt(m) !== 38 || m + 1 >= g) return !1;
-        if (a = e.src.charCodeAt(m + 1), a === 35) {
-            if (c = e.src.slice(m).match(Jm), c) return i || (l = c[1][0].toLowerCase() === "x" ? parseInt(c[1].slice(1), 16) : parseInt(c[1], 10), d = e.push("text_special", "", 0), d.content = Xm(l) ? Ac(l) : Ac(65533), d.markup = c[0], d.info = "entity"), e.pos += c[0].length, !0
-        } else if (c = e.src.slice(m).match(Km), c && Zm(Tc, c[1])) return i || (d = e.push("text_special", "", 0), d.content = Tc[c[1]], d.markup = c[0], d.info = "entity"), e.pos += c[0].length, !0;
+        if (e.src.charCodeAt(f) !== 38 || f + 1 >= g) return !1;
+        if (a = e.src.charCodeAt(f + 1), a === 35) {
+            if (c = e.src.slice(f).match(rp), c) return i || (l = c[1][0].toLowerCase() === "x" ? parseInt(c[1].slice(1), 16) : parseInt(c[1], 10), d = e.push("text_special", "", 0), d.content = tp(l) ? Mc(l) : Mc(65533), d.markup = c[0], d.info = "entity"), e.pos += c[0].length, !0
+        } else if (c = e.src.slice(f).match(np), c && ep(qc, c[1])) return i || (d = e.push("text_special", "", 0), d.content = qc[c[1]], d.markup = c[0], d.info = "entity"), e.pos += c[0].length, !0;
         return !1
     }
 });
-var zc = W((D2, Dc) => {
+var Fc = W((H2, Rc) => {
     "use strict";
 
-    function Ec(r) {
-        var e, i, a, l, c, d, m, g, y = {},
+    function zc(r) {
+        var e, i, a, l, c, d, f, g, y = {},
             _ = r.length;
         if (_) {
-            var k = 0,
+            var w = 0,
                 T = -2,
                 A = [];
             for (e = 0; e < _; e++)
-                if (a = r[e], A.push(0), (r[k].marker !== a.marker || T !== a.token - 1) && (k = e), T = a.token, a.length = a.length || 0, !!a.close) {
-                    for (y.hasOwnProperty(a.marker) || (y[a.marker] = [-1, -1, -1, -1, -1, -1]), c = y[a.marker][(a.open ? 3 : 0) + a.length % 3], i = k - A[k] - 1, d = i; i > c; i -= A[i] + 1)
-                        if (l = r[i], l.marker === a.marker && l.open && l.end < 0 && (m = !1, (l.close || a.open) && (l.length + a.length) % 3 === 0 && (l.length % 3 !== 0 || a.length % 3 !== 0) && (m = !0), !m)) {
+                if (a = r[e], A.push(0), (r[w].marker !== a.marker || T !== a.token - 1) && (w = e), T = a.token, a.length = a.length || 0, !!a.close) {
+                    for (y.hasOwnProperty(a.marker) || (y[a.marker] = [-1, -1, -1, -1, -1, -1]), c = y[a.marker][(a.open ? 3 : 0) + a.length % 3], i = w - A[w] - 1, d = i; i > c; i -= A[i] + 1)
+                        if (l = r[i], l.marker === a.marker && l.open && l.end < 0 && (f = !1, (l.close || a.open) && (l.length + a.length) % 3 === 0 && (l.length % 3 !== 0 || a.length % 3 !== 0) && (f = !0), !f)) {
                             g = i > 0 && !r[i - 1].open ? A[i - 1] + 1 : 0, A[e] = e - i + g, A[i] = g, a.open = !1, l.end = e, l.close = !1, d = -1, T = -2;
                             break
                         } d !== -1 && (y[a.marker][(a.open ? 3 : 0) + (a.length || 0) % 3] = d)
                 }
         }
     }
-    Dc.exports = function(e) {
+    Rc.exports = function(e) {
         var i, a = e.tokens_meta,
             l = e.tokens_meta.length;
-        for (Ec(e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && Ec(a[i].delimiters)
+        for (zc(e.delimiters), i = 0; i < l; i++) a[i] && a[i].delimiters && zc(a[i].delimiters)
     }
 });
-var Fc = W((z2, Rc) => {
+var Nc = W(($2, Bc) => {
     "use strict";
-    Rc.exports = function(e) {
+    Bc.exports = function(e) {
         var i, a, l = 0,
             c = e.tokens,
             d = e.tokens.length;
         for (i = a = 0; i < d; i++) c[i].nesting < 0 && l--, c[i].level = l, c[i].nesting > 0 && l++, c[i].type === "text" && i + 1 < d && c[i + 1].type === "text" ? c[i + 1].content = c[i].content + c[i + 1].content : (i !== a && (c[a] = c[i]), a++);
         i !== a && (c.length = a)
     }
 });
-var Ic = W((R2, Pc) => {
+var Hc = W((G2, Oc) => {
     "use strict";
-    var yi = z0(),
-        Bc = Se().isWhiteSpace,
-        Nc = Se().isPunctChar,
-        Lc = Se().isMdAsciiPunct;
+    var ki = R0(),
+        Lc = Se().isWhiteSpace,
+        Pc = Se().isPunctChar,
+        Ic = Se().isMdAsciiPunct;
 
     function Lr(r, e, i, a) {
         this.src = r, this.env = i, this.md = e, this.tokens = a, this.tokens_meta = Array(a.length), this.pos = 0, this.posMax = this.src.length, this.level = 0, this.pending = "", this.pendingLevel = 0, this.cache = {}, this.delimiters = [], this._prev_delimiters = [], this.backticks = {}, this.backticksScanned = !1, this.linkLevel = 0
     }
     Lr.prototype.pushPending = function() {
-        var r = new yi("text", "", 0);
+        var r = new ki("text", "", 0);
         return r.content = this.pending, r.level = this.pendingLevel, this.tokens.push(r), this.pending = "", r
     };
     Lr.prototype.push = function(r, e, i) {
         this.pending && this.pushPending();
-        var a = new yi(r, e, i),
+        var a = new ki(r, e, i),
             l = null;
         return i < 0 && (this.level--, this.delimiters = this._prev_delimiters.pop()), a.level = this.level, i > 0 && (this.level++, this._prev_delimiters.push(this.delimiters), this.delimiters = [], l = {
             delimiters: this.delimiters
         }), this.pendingLevel = this.level, this.tokens.push(a), this.tokens_meta.push(l), a
     };
     Lr.prototype.scanDelims = function(r, e) {
         var i = r,
-            a, l, c, d, m, g, y, _, k, T = !0,
+            a, l, c, d, f, g, y, _, w, T = !0,
             A = !0,
             L = this.posMax,
             R = this.src.charCodeAt(r);
         for (a = r > 0 ? this.src.charCodeAt(r - 1) : 32; i < L && this.src.charCodeAt(i) === R;) i++;
-        return c = i - r, l = i < L ? this.src.charCodeAt(i) : 32, y = Lc(a) || Nc(String.fromCharCode(a)), k = Lc(l) || Nc(String.fromCharCode(l)), g = Bc(a), _ = Bc(l), _ ? T = !1 : k && (g || y || (T = !1)), g ? A = !1 : y && (_ || k || (A = !1)), e ? (d = T, m = A) : (d = T && (!A || y), m = A && (!T || k)), {
+        return c = i - r, l = i < L ? this.src.charCodeAt(i) : 32, y = Ic(a) || Pc(String.fromCharCode(a)), w = Ic(l) || Pc(String.fromCharCode(l)), g = Lc(a), _ = Lc(l), _ ? T = !1 : w && (g || y || (T = !1)), g ? A = !1 : y && (_ || w || (A = !1)), e ? (d = T, f = A) : (d = T && (!A || y), f = A && (!T || w)), {
             can_open: d,
-            can_close: m,
+            can_close: f,
             length: c
         }
     };
-    Lr.prototype.Token = yi;
-    Pc.exports = Lr
+    Lr.prototype.Token = ki;
+    Oc.exports = Lr
 });
-var $c = W((F2, Hc) => {
+var Vc = W((V2, Gc) => {
     "use strict";
-    var Oc = E0(),
-        xi = [
-            ["text", sc()],
-            ["linkify", cc()],
-            ["newline", hc()],
-            ["escape", mc()],
-            ["backticks", fc()],
-            ["strikethrough", mi().tokenize],
-            ["emphasis", fi().tokenize],
-            ["link", xc()],
-            ["image", wc()],
-            ["autolink", _c()],
-            ["html_inline", Cc()],
-            ["entity", Mc()]
+    var $c = D0(),
+        _i = [
+            ["text", cc()],
+            ["linkify", hc()],
+            ["newline", mc()],
+            ["escape", fc()],
+            ["backticks", bc()],
+            ["strikethrough", bi().tokenize],
+            ["emphasis", xi().tokenize],
+            ["link", wc()],
+            ["image", _c()],
+            ["autolink", Cc()],
+            ["html_inline", Ac()],
+            ["entity", Dc()]
         ],
-        vi = [
-            ["balance_pairs", zc()],
-            ["strikethrough", mi().postProcess],
-            ["emphasis", fi().postProcess],
-            ["fragments_join", Fc()]
+        Si = [
+            ["balance_pairs", Fc()],
+            ["strikethrough", bi().postProcess],
+            ["emphasis", xi().postProcess],
+            ["fragments_join", Nc()]
         ];
 
     function Pr() {
         var r;
-        for (this.ruler = new Oc, r = 0; r < xi.length; r++) this.ruler.push(xi[r][0], xi[r][1]);
-        for (this.ruler2 = new Oc, r = 0; r < vi.length; r++) this.ruler2.push(vi[r][0], vi[r][1])
+        for (this.ruler = new $c, r = 0; r < _i.length; r++) this.ruler.push(_i[r][0], _i[r][1]);
+        for (this.ruler2 = new $c, r = 0; r < Si.length; r++) this.ruler2.push(Si[r][0], Si[r][1])
     }
     Pr.prototype.skipToken = function(r) {
         var e, i, a = r.pos,
             l = this.ruler.getRules(""),
             c = l.length,
             d = r.md.options.maxNesting,
-            m = r.cache;
-        if (typeof m[a] < "u") {
-            r.pos = m[a];
+            f = r.cache;
+        if (typeof f[a] < "u") {
+            r.pos = f[a];
             return
         }
         if (r.level < d) {
             for (i = 0; i < c; i++)
                 if (r.level++, e = l[i](r, !0), r.level--, e) {
                     if (a >= r.pos) throw new Error("inline rule didn't increment state.pos");
                     break
                 }
         } else r.pos = r.posMax;
-        e || r.pos++, m[a] = r.pos
+        e || r.pos++, f[a] = r.pos
     };
     Pr.prototype.tokenize = function(r) {
-        for (var e, i, a, l = this.ruler.getRules(""), c = l.length, d = r.posMax, m = r.md.options.maxNesting; r.pos < d;) {
-            if (a = r.pos, r.level < m) {
+        for (var e, i, a, l = this.ruler.getRules(""), c = l.length, d = r.posMax, f = r.md.options.maxNesting; r.pos < d;) {
+            if (a = r.pos, r.level < f) {
                 for (i = 0; i < c; i++)
                     if (e = l[i](r, !1), e) {
                         if (a >= r.pos) throw new Error("inline rule didn't increment state.pos");
                         break
                     }
             }
             if (e) {
@@ -5110,76 +5110,76 @@
                 continue
             }
             r.pending += r.src[r.pos++]
         }
         r.pending && r.pushPending()
     };
     Pr.prototype.parse = function(r, e, i, a) {
-        var l, c, d, m = new this.State(r, e, i, a);
-        for (this.tokenize(m), c = this.ruler2.getRules(""), d = c.length, l = 0; l < d; l++) c[l](m)
+        var l, c, d, f = new this.State(r, e, i, a);
+        for (this.tokenize(f), c = this.ruler2.getRules(""), d = c.length, l = 0; l < d; l++) c[l](f)
     };
-    Pr.prototype.State = Ic();
-    Hc.exports = Pr
+    Pr.prototype.State = Hc();
+    Gc.exports = Pr
 });
-var Vc = W((B2, Gc) => {
+var Uc = W((j2, jc) => {
     "use strict";
-    Gc.exports = function(r) {
+    jc.exports = function(r) {
         var e = {};
-        r = r || {}, e.src_Any = ti().source, e.src_Cc = ri().source, e.src_Z = ni().source, e.src_P = C0().source, e.src_ZPCc = [e.src_Z, e.src_P, e.src_Cc].join("|"), e.src_ZCc = [e.src_Z, e.src_Cc].join("|");
+        r = r || {}, e.src_Any = oi().source, e.src_Cc = ai().source, e.src_Z = si().source, e.src_P = T0().source, e.src_ZPCc = [e.src_Z, e.src_P, e.src_Cc].join("|"), e.src_ZCc = [e.src_Z, e.src_Cc].join("|");
         var i = "[><\uFF5C]";
         return e.src_pseudo_letter = "(?:(?!" + i + "|" + e.src_ZPCc + ")" + e.src_Any + ")", e.src_ip4 = "(?:(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.){3}(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)", e.src_auth = "(?:(?:(?!" + e.src_ZCc + "|[@/\\[\\]()]).)+@)?", e.src_port = "(?::(?:6(?:[0-4]\\d{3}|5(?:[0-4]\\d{2}|5(?:[0-2]\\d|3[0-5])))|[1-5]?\\d{1,4}))?", e.src_host_terminator = "(?=$|" + i + "|" + e.src_ZPCc + ")(?!" + (r["---"] ? "-(?!--)|" : "-|") + "_|:\\d|\\.-|\\.(?!$|" + e.src_ZPCc + "))", e.src_path = "(?:[/?#](?:(?!" + e.src_ZCc + "|" + i + `|[()[\\]{}.,"'?!\\-;]).|\\[(?:(?!` + e.src_ZCc + "|\\]).)*\\]|\\((?:(?!" + e.src_ZCc + "|[)]).)*\\)|\\{(?:(?!" + e.src_ZCc + '|[}]).)*\\}|\\"(?:(?!' + e.src_ZCc + `|["]).)+\\"|\\'(?:(?!` + e.src_ZCc + "|[']).)+\\'|\\'(?=" + e.src_pseudo_letter + "|[-])|\\.{2,}[a-zA-Z0-9%/&]|\\.(?!" + e.src_ZCc + "|[.]|$)|" + (r["---"] ? "\\-(?!--(?:[^-]|$))(?:-*)|" : "\\-+|") + ",(?!" + e.src_ZCc + "|$)|;(?!" + e.src_ZCc + "|$)|\\!+(?!" + e.src_ZCc + "|[!]|$)|\\?(?!" + e.src_ZCc + "|[?]|$))+|\\/)?", e.src_email_name = '[\\-;:&=\\+\\$,\\.a-zA-Z0-9_][\\-;:&=\\+\\$,\\"\\.a-zA-Z0-9_]*', e.src_xn = "xn--[a-z0-9\\-]{1,59}", e.src_domain_root = "(?:" + e.src_xn + "|" + e.src_pseudo_letter + "{1,63})", e.src_domain = "(?:" + e.src_xn + "|(?:" + e.src_pseudo_letter + ")|(?:" + e.src_pseudo_letter + "(?:-|" + e.src_pseudo_letter + "){0,61}" + e.src_pseudo_letter + "))", e.src_host = "(?:(?:(?:(?:" + e.src_domain + ")\\.)*" + e.src_domain + "))", e.tpl_host_fuzzy = "(?:" + e.src_ip4 + "|(?:(?:(?:" + e.src_domain + ")\\.)+(?:%TLDS%)))", e.tpl_host_no_ip_fuzzy = "(?:(?:(?:" + e.src_domain + ")\\.)+(?:%TLDS%))", e.src_host_strict = e.src_host + e.src_host_terminator, e.tpl_host_fuzzy_strict = e.tpl_host_fuzzy + e.src_host_terminator, e.src_host_port_strict = e.src_host + e.src_port + e.src_host_terminator, e.tpl_host_port_fuzzy_strict = e.tpl_host_fuzzy + e.src_port + e.src_host_terminator, e.tpl_host_port_no_ip_fuzzy_strict = e.tpl_host_no_ip_fuzzy + e.src_port + e.src_host_terminator, e.tpl_host_fuzzy_test = "localhost|www\\.|\\.\\d{1,3}\\.|(?:\\.(?:%TLDS%)(?:" + e.src_ZPCc + "|>|$))", e.tpl_email_fuzzy = "(^|" + i + '|"|\\(|' + e.src_ZCc + ")(" + e.src_email_name + "@" + e.tpl_host_fuzzy_strict + ")", e.tpl_link_fuzzy = "(^|(?![.:/\\-_@])(?:[$+<=>^`|\uFF5C]|" + e.src_ZPCc + "))((?![$+<=>^`|\uFF5C])" + e.tpl_host_port_fuzzy_strict + e.src_path + ")", e.tpl_link_no_ip_fuzzy = "(^|(?![.:/\\-_@])(?:[$+<=>^`|\uFF5C]|" + e.src_ZPCc + "))((?![$+<=>^`|\uFF5C])" + e.tpl_host_port_no_ip_fuzzy_strict + e.src_path + ")", e
     }
 });
-var Qc = W((N2, Yc) => {
+var Xc = W((U2, Qc) => {
     "use strict";
 
-    function wi(r) {
+    function Ci(r) {
         var e = Array.prototype.slice.call(arguments, 1);
         return e.forEach(function(i) {
             i && Object.keys(i).forEach(function(a) {
                 r[a] = i[a]
             })
         }), r
     }
 
-    function P0(r) {
+    function I0(r) {
         return Object.prototype.toString.call(r)
     }
 
-    function ep(r) {
-        return P0(r) === "[object String]"
+    function ip(r) {
+        return I0(r) === "[object String]"
     }
 
-    function tp(r) {
-        return P0(r) === "[object Object]"
+    function op(r) {
+        return I0(r) === "[object Object]"
     }
 
-    function rp(r) {
-        return P0(r) === "[object RegExp]"
+    function ap(r) {
+        return I0(r) === "[object RegExp]"
     }
 
-    function jc(r) {
-        return P0(r) === "[object Function]"
+    function Wc(r) {
+        return I0(r) === "[object Function]"
     }
 
-    function np(r) {
+    function sp(r) {
         return r.replace(/[.?*+^$[\]\\(){}|-]/g, "\\$&")
     }
-    var Wc = {
+    var Zc = {
         fuzzyLink: !0,
         fuzzyEmail: !0,
         fuzzyIP: !1
     };
 
-    function ip(r) {
+    function lp(r) {
         return Object.keys(r || {}).reduce(function(e, i) {
-            return e || Wc.hasOwnProperty(i)
+            return e || Zc.hasOwnProperty(i)
         }, !1)
     }
-    var op = {
+    var cp = {
             "http:": {
                 validate: function(r, e, i) {
                     var a = r.slice(e);
                     return i.re.http || (i.re.http = new RegExp("^\\/\\/" + i.re.src_auth + i.re.src_host_port_strict + i.re.src_path, "i")), i.re.http.test(a) ? a.match(i.re.http)[0].length : 0
                 }
             },
             "https:": "http:",
@@ -5193,285 +5193,285 @@
             "mailto:": {
                 validate: function(r, e, i) {
                     var a = r.slice(e);
                     return i.re.mailto || (i.re.mailto = new RegExp("^" + i.re.src_email_name + "@" + i.re.src_host_strict, "i")), i.re.mailto.test(a) ? a.match(i.re.mailto)[0].length : 0
                 }
             }
         },
-        ap = "a[cdefgilmnoqrstuwxz]|b[abdefghijmnorstvwyz]|c[acdfghiklmnoruvwxyz]|d[ejkmoz]|e[cegrstu]|f[ijkmor]|g[abdefghilmnpqrstuwy]|h[kmnrtu]|i[delmnoqrst]|j[emop]|k[eghimnprwyz]|l[abcikrstuvy]|m[acdeghklmnopqrstuvwxyz]|n[acefgilopruz]|om|p[aefghklmnrstwy]|qa|r[eosuw]|s[abcdeghijklmnortuvxyz]|t[cdfghjklmnortvwz]|u[agksyz]|v[aceginu]|w[fs]|y[et]|z[amw]",
-        sp = "biz|com|edu|gov|net|org|pro|web|xxx|aero|asia|coop|info|museum|name|shop|\u0440\u0444".split("|");
+        up = "a[cdefgilmnoqrstuwxz]|b[abdefghijmnorstvwyz]|c[acdfghiklmnoruvwxyz]|d[ejkmoz]|e[cegrstu]|f[ijkmor]|g[abdefghilmnpqrstuwy]|h[kmnrtu]|i[delmnoqrst]|j[emop]|k[eghimnprwyz]|l[abcikrstuvy]|m[acdeghklmnopqrstuvwxyz]|n[acefgilopruz]|om|p[aefghklmnrstwy]|qa|r[eosuw]|s[abcdeghijklmnortuvxyz]|t[cdfghjklmnortvwz]|u[agksyz]|v[aceginu]|w[fs]|y[et]|z[amw]",
+        hp = "biz|com|edu|gov|net|org|pro|web|xxx|aero|asia|coop|info|museum|name|shop|\u0440\u0444".split("|");
 
-    function lp(r) {
+    function dp(r) {
         r.__index__ = -1, r.__text_cache__ = ""
     }
 
-    function cp(r) {
+    function mp(r) {
         return function(e, i) {
             var a = e.slice(i);
             return r.test(a) ? a.match(r)[0].length : 0
         }
     }
 
-    function Uc() {
+    function Yc() {
         return function(r, e) {
             e.normalize(r)
         }
     }
 
-    function L0(r) {
-        var e = r.re = Vc()(r.__opts__),
+    function P0(r) {
+        var e = r.re = Uc()(r.__opts__),
             i = r.__tlds__.slice();
-        r.onCompile(), r.__tlds_replaced__ || i.push(ap), i.push(e.src_xn), e.src_tlds = i.join("|");
+        r.onCompile(), r.__tlds_replaced__ || i.push(up), i.push(e.src_xn), e.src_tlds = i.join("|");
 
-        function a(m) {
-            return m.replace("%TLDS%", e.src_tlds)
+        function a(f) {
+            return f.replace("%TLDS%", e.src_tlds)
         }
         e.email_fuzzy = RegExp(a(e.tpl_email_fuzzy), "i"), e.link_fuzzy = RegExp(a(e.tpl_link_fuzzy), "i"), e.link_no_ip_fuzzy = RegExp(a(e.tpl_link_no_ip_fuzzy), "i"), e.host_fuzzy_test = RegExp(a(e.tpl_host_fuzzy_test), "i");
         var l = [];
         r.__compiled__ = {};
 
-        function c(m, g) {
-            throw new Error('(LinkifyIt) Invalid schema "' + m + '": ' + g)
+        function c(f, g) {
+            throw new Error('(LinkifyIt) Invalid schema "' + f + '": ' + g)
         }
-        Object.keys(r.__schemas__).forEach(function(m) {
-            var g = r.__schemas__[m];
+        Object.keys(r.__schemas__).forEach(function(f) {
+            var g = r.__schemas__[f];
             if (g !== null) {
                 var y = {
                     validate: null,
                     link: null
                 };
-                if (r.__compiled__[m] = y, tp(g)) {
-                    rp(g.validate) ? y.validate = cp(g.validate) : jc(g.validate) ? y.validate = g.validate : c(m, g), jc(g.normalize) ? y.normalize = g.normalize : g.normalize ? c(m, g) : y.normalize = Uc();
+                if (r.__compiled__[f] = y, op(g)) {
+                    ap(g.validate) ? y.validate = mp(g.validate) : Wc(g.validate) ? y.validate = g.validate : c(f, g), Wc(g.normalize) ? y.normalize = g.normalize : g.normalize ? c(f, g) : y.normalize = Yc();
                     return
                 }
-                if (ep(g)) {
-                    l.push(m);
+                if (ip(g)) {
+                    l.push(f);
                     return
                 }
-                c(m, g)
+                c(f, g)
             }
-        }), l.forEach(function(m) {
-            r.__compiled__[r.__schemas__[m]] && (r.__compiled__[m].validate = r.__compiled__[r.__schemas__[m]].validate, r.__compiled__[m].normalize = r.__compiled__[r.__schemas__[m]].normalize)
+        }), l.forEach(function(f) {
+            r.__compiled__[r.__schemas__[f]] && (r.__compiled__[f].validate = r.__compiled__[r.__schemas__[f]].validate, r.__compiled__[f].normalize = r.__compiled__[r.__schemas__[f]].normalize)
         }), r.__compiled__[""] = {
             validate: null,
-            normalize: Uc()
+            normalize: Yc()
         };
-        var d = Object.keys(r.__compiled__).filter(function(m) {
-            return m.length > 0 && r.__compiled__[m]
-        }).map(np).join("|");
-        r.re.schema_test = RegExp("(^|(?!_)(?:[><\uFF5C]|" + e.src_ZPCc + "))(" + d + ")", "i"), r.re.schema_search = RegExp("(^|(?!_)(?:[><\uFF5C]|" + e.src_ZPCc + "))(" + d + ")", "ig"), r.re.schema_at_start = RegExp("^" + r.re.schema_search.source, "i"), r.re.pretest = RegExp("(" + r.re.schema_test.source + ")|(" + r.re.host_fuzzy_test.source + ")|@", "i"), lp(r)
+        var d = Object.keys(r.__compiled__).filter(function(f) {
+            return f.length > 0 && r.__compiled__[f]
+        }).map(sp).join("|");
+        r.re.schema_test = RegExp("(^|(?!_)(?:[><\uFF5C]|" + e.src_ZPCc + "))(" + d + ")", "i"), r.re.schema_search = RegExp("(^|(?!_)(?:[><\uFF5C]|" + e.src_ZPCc + "))(" + d + ")", "ig"), r.re.schema_at_start = RegExp("^" + r.re.schema_search.source, "i"), r.re.pretest = RegExp("(" + r.re.schema_test.source + ")|(" + r.re.host_fuzzy_test.source + ")|@", "i"), dp(r)
     }
 
-    function up(r, e) {
+    function pp(r, e) {
         var i = r.__index__,
             a = r.__last_index__,
             l = r.__text_cache__.slice(i, a);
         this.schema = r.__schema__.toLowerCase(), this.index = i + e, this.lastIndex = a + e, this.raw = l, this.text = l, this.url = l
     }
 
-    function ki(r, e) {
-        var i = new up(r, e);
+    function Ti(r, e) {
+        var i = new pp(r, e);
         return r.__compiled__[i.schema].normalize(i, r), i
     }
 
     function lt(r, e) {
         if (!(this instanceof lt)) return new lt(r, e);
-        e || ip(r) && (e = r, r = {}), this.__opts__ = wi({}, Wc, e), this.__index__ = -1, this.__last_index__ = -1, this.__schema__ = "", this.__text_cache__ = "", this.__schemas__ = wi({}, op, r), this.__compiled__ = {}, this.__tlds__ = sp, this.__tlds_replaced__ = !1, this.re = {}, L0(this)
+        e || lp(r) && (e = r, r = {}), this.__opts__ = Ci({}, Zc, e), this.__index__ = -1, this.__last_index__ = -1, this.__schema__ = "", this.__text_cache__ = "", this.__schemas__ = Ci({}, cp, r), this.__compiled__ = {}, this.__tlds__ = hp, this.__tlds_replaced__ = !1, this.re = {}, P0(this)
     }
     lt.prototype.add = function(e, i) {
-        return this.__schemas__[e] = i, L0(this), this
+        return this.__schemas__[e] = i, P0(this), this
     };
     lt.prototype.set = function(e) {
-        return this.__opts__ = wi(this.__opts__, e), this
+        return this.__opts__ = Ci(this.__opts__, e), this
     };
     lt.prototype.test = function(e) {
         if (this.__text_cache__ = e, this.__index__ = -1, !e.length) return !1;
-        var i, a, l, c, d, m, g, y, _;
+        var i, a, l, c, d, f, g, y, _;
         if (this.re.schema_test.test(e)) {
             for (g = this.re.schema_search, g.lastIndex = 0;
                 (i = g.exec(e)) !== null;)
                 if (c = this.testSchemaAt(e, i[2], g.lastIndex), c) {
                     this.__schema__ = i[2], this.__index__ = i.index + i[1].length, this.__last_index__ = i.index + i[0].length + c;
                     break
                 }
         }
-        return this.__opts__.fuzzyLink && this.__compiled__["http:"] && (y = e.search(this.re.host_fuzzy_test), y >= 0 && (this.__index__ < 0 || y < this.__index__) && (a = e.match(this.__opts__.fuzzyIP ? this.re.link_fuzzy : this.re.link_no_ip_fuzzy)) !== null && (d = a.index + a[1].length, (this.__index__ < 0 || d < this.__index__) && (this.__schema__ = "", this.__index__ = d, this.__last_index__ = a.index + a[0].length))), this.__opts__.fuzzyEmail && this.__compiled__["mailto:"] && (_ = e.indexOf("@"), _ >= 0 && (l = e.match(this.re.email_fuzzy)) !== null && (d = l.index + l[1].length, m = l.index + l[0].length, (this.__index__ < 0 || d < this.__index__ || d === this.__index__ && m > this.__last_index__) && (this.__schema__ = "mailto:", this.__index__ = d, this.__last_index__ = m))), this.__index__ >= 0
+        return this.__opts__.fuzzyLink && this.__compiled__["http:"] && (y = e.search(this.re.host_fuzzy_test), y >= 0 && (this.__index__ < 0 || y < this.__index__) && (a = e.match(this.__opts__.fuzzyIP ? this.re.link_fuzzy : this.re.link_no_ip_fuzzy)) !== null && (d = a.index + a[1].length, (this.__index__ < 0 || d < this.__index__) && (this.__schema__ = "", this.__index__ = d, this.__last_index__ = a.index + a[0].length))), this.__opts__.fuzzyEmail && this.__compiled__["mailto:"] && (_ = e.indexOf("@"), _ >= 0 && (l = e.match(this.re.email_fuzzy)) !== null && (d = l.index + l[1].length, f = l.index + l[0].length, (this.__index__ < 0 || d < this.__index__ || d === this.__index__ && f > this.__last_index__) && (this.__schema__ = "mailto:", this.__index__ = d, this.__last_index__ = f))), this.__index__ >= 0
     };
     lt.prototype.pretest = function(e) {
         return this.re.pretest.test(e)
     };
     lt.prototype.testSchemaAt = function(e, i, a) {
         return this.__compiled__[i.toLowerCase()] ? this.__compiled__[i.toLowerCase()].validate(e, a, this) : 0
     };
     lt.prototype.match = function(e) {
         var i = 0,
             a = [];
-        this.__index__ >= 0 && this.__text_cache__ === e && (a.push(ki(this, i)), i = this.__last_index__);
-        for (var l = i ? e.slice(i) : e; this.test(l);) a.push(ki(this, i)), l = l.slice(this.__last_index__), i += this.__last_index__;
+        this.__index__ >= 0 && this.__text_cache__ === e && (a.push(Ti(this, i)), i = this.__last_index__);
+        for (var l = i ? e.slice(i) : e; this.test(l);) a.push(Ti(this, i)), l = l.slice(this.__last_index__), i += this.__last_index__;
         return a.length ? a : null
     };
     lt.prototype.matchAtStart = function(e) {
         if (this.__text_cache__ = e, this.__index__ = -1, !e.length) return null;
         var i = this.re.schema_at_start.exec(e);
         if (!i) return null;
         var a = this.testSchemaAt(e, i[2], i[0].length);
-        return a ? (this.__schema__ = i[2], this.__index__ = i.index + i[1].length, this.__last_index__ = i.index + i[0].length + a, ki(this, 0)) : null
+        return a ? (this.__schema__ = i[2], this.__index__ = i.index + i[1].length, this.__last_index__ = i.index + i[0].length + a, Ti(this, 0)) : null
     };
     lt.prototype.tlds = function(e, i) {
         return e = Array.isArray(e) ? e : [e], i ? (this.__tlds__ = this.__tlds__.concat(e).sort().filter(function(a, l, c) {
             return a !== c[l - 1]
-        }).reverse(), L0(this), this) : (this.__tlds__ = e.slice(), this.__tlds_replaced__ = !0, L0(this), this)
+        }).reverse(), P0(this), this) : (this.__tlds__ = e.slice(), this.__tlds_replaced__ = !0, P0(this), this)
     };
     lt.prototype.normalize = function(e) {
         e.schema || (e.url = "http://" + e.url), e.schema === "mailto:" && !/^mailto:/i.test(e.url) && (e.url = "mailto:" + e.url)
     };
     lt.prototype.onCompile = function() {};
-    Yc.exports = lt
+    Qc.exports = lt
 });
-var iu = W((L2, nu) => {
+var au = W((W2, ou) => {
     "use strict";
-    var Xc = "-",
-        hp = /^xn--/,
-        dp = /[^\0-\x7F]/,
-        mp = /[\x2E\u3002\uFF0E\uFF61]/g,
-        pp = {
+    var Kc = "-",
+        fp = /^xn--/,
+        gp = /[^\0-\x7F]/,
+        bp = /[\x2E\u3002\uFF0E\uFF61]/g,
+        yp = {
             overflow: "Overflow: input needs wider integers to process",
             "not-basic": "Illegal input >= 0x80 (not a basic code point)",
             "invalid-input": "Invalid input"
         },
-        _i = 35,
+        Ai = 35,
         At = Math.floor,
-        Si = String.fromCharCode;
+        qi = String.fromCharCode;
 
-    function Zt(r) {
-        throw new RangeError(pp[r])
+    function Xt(r) {
+        throw new RangeError(yp[r])
     }
 
-    function fp(r, e) {
+    function xp(r, e) {
         let i = [],
             a = r.length;
         for (; a--;) i[a] = e(r[a]);
         return i
     }
 
-    function Jc(r, e) {
+    function eu(r, e) {
         let i = r.split("@"),
             a = "";
-        i.length > 1 && (a = i[0] + "@", r = i[1]), r = r.replace(mp, ".");
+        i.length > 1 && (a = i[0] + "@", r = i[1]), r = r.replace(bp, ".");
         let l = r.split("."),
-            c = fp(l, e).join(".");
+            c = xp(l, e).join(".");
         return a + c
     }
 
-    function Kc(r) {
+    function tu(r) {
         let e = [],
             i = 0,
             a = r.length;
         for (; i < a;) {
             let l = r.charCodeAt(i++);
             if (l >= 55296 && l <= 56319 && i < a) {
                 let c = r.charCodeAt(i++);
                 (c & 64512) == 56320 ? e.push(((l & 1023) << 10) + (c & 1023) + 65536) : (e.push(l), i--)
             } else e.push(l)
         }
         return e
     }
-    var gp = r => String.fromCodePoint(...r),
-        bp = function(r) {
+    var vp = r => String.fromCodePoint(...r),
+        wp = function(r) {
             return r >= 48 && r < 58 ? 26 + (r - 48) : r >= 65 && r < 91 ? r - 65 : r >= 97 && r < 123 ? r - 97 : 36
         },
-        Zc = function(r, e) {
+        Jc = function(r, e) {
             return r + 22 + 75 * (r < 26) - ((e != 0) << 5)
         },
-        eu = function(r, e, i) {
+        ru = function(r, e, i) {
             let a = 0;
-            for (r = i ? At(r / 700) : r >> 1, r += At(r / e); r > _i * 26 >> 1; a += 36) r = At(r / _i);
-            return At(a + (_i + 1) * r / (r + 38))
+            for (r = i ? At(r / 700) : r >> 1, r += At(r / e); r > Ai * 26 >> 1; a += 36) r = At(r / Ai);
+            return At(a + (Ai + 1) * r / (r + 38))
         },
-        tu = function(r) {
+        nu = function(r) {
             let e = [],
                 i = r.length,
                 a = 0,
                 l = 128,
                 c = 72,
-                d = r.lastIndexOf(Xc);
+                d = r.lastIndexOf(Kc);
             d < 0 && (d = 0);
-            for (let m = 0; m < d; ++m) r.charCodeAt(m) >= 128 && Zt("not-basic"), e.push(r.charCodeAt(m));
-            for (let m = d > 0 ? d + 1 : 0; m < i;) {
+            for (let f = 0; f < d; ++f) r.charCodeAt(f) >= 128 && Xt("not-basic"), e.push(r.charCodeAt(f));
+            for (let f = d > 0 ? d + 1 : 0; f < i;) {
                 let g = a;
-                for (let _ = 1, k = 36;; k += 36) {
-                    m >= i && Zt("invalid-input");
-                    let T = bp(r.charCodeAt(m++));
-                    T >= 36 && Zt("invalid-input"), T > At((2147483647 - a) / _) && Zt("overflow"), a += T * _;
-                    let A = k <= c ? 1 : k >= c + 26 ? 26 : k - c;
+                for (let _ = 1, w = 36;; w += 36) {
+                    f >= i && Xt("invalid-input");
+                    let T = wp(r.charCodeAt(f++));
+                    T >= 36 && Xt("invalid-input"), T > At((2147483647 - a) / _) && Xt("overflow"), a += T * _;
+                    let A = w <= c ? 1 : w >= c + 26 ? 26 : w - c;
                     if (T < A) break;
                     let L = 36 - A;
-                    _ > At(2147483647 / L) && Zt("overflow"), _ *= L
+                    _ > At(2147483647 / L) && Xt("overflow"), _ *= L
                 }
                 let y = e.length + 1;
-                c = eu(a - g, y, g == 0), At(a / y) > 2147483647 - l && Zt("overflow"), l += At(a / y), a %= y, e.splice(a++, 0, l)
+                c = ru(a - g, y, g == 0), At(a / y) > 2147483647 - l && Xt("overflow"), l += At(a / y), a %= y, e.splice(a++, 0, l)
             }
             return String.fromCodePoint(...e)
         },
-        ru = function(r) {
+        iu = function(r) {
             let e = [];
-            r = Kc(r);
+            r = tu(r);
             let i = r.length,
                 a = 128,
                 l = 0,
                 c = 72;
-            for (let g of r) g < 128 && e.push(Si(g));
+            for (let g of r) g < 128 && e.push(qi(g));
             let d = e.length,
-                m = d;
-            for (d && e.push(Xc); m < i;) {
+                f = d;
+            for (d && e.push(Kc); f < i;) {
                 let g = 2147483647;
                 for (let _ of r) _ >= a && _ < g && (g = _);
-                let y = m + 1;
-                g - a > At((2147483647 - l) / y) && Zt("overflow"), l += (g - a) * y, a = g;
+                let y = f + 1;
+                g - a > At((2147483647 - l) / y) && Xt("overflow"), l += (g - a) * y, a = g;
                 for (let _ of r)
-                    if (_ < a && ++l > 2147483647 && Zt("overflow"), _ === a) {
-                        let k = l;
+                    if (_ < a && ++l > 2147483647 && Xt("overflow"), _ === a) {
+                        let w = l;
                         for (let T = 36;; T += 36) {
                             let A = T <= c ? 1 : T >= c + 26 ? 26 : T - c;
-                            if (k < A) break;
-                            let L = k - A,
+                            if (w < A) break;
+                            let L = w - A,
                                 R = 36 - A;
-                            e.push(Si(Zc(A + L % R, 0))), k = At(L / R)
+                            e.push(qi(Jc(A + L % R, 0))), w = At(L / R)
                         }
-                        e.push(Si(Zc(k, 0))), c = eu(l, y, m === d), l = 0, ++m
+                        e.push(qi(Jc(w, 0))), c = ru(l, y, f === d), l = 0, ++f
                     }++ l, ++a
             }
             return e.join("")
         },
-        yp = function(r) {
-            return Jc(r, function(e) {
-                return hp.test(e) ? tu(e.slice(4).toLowerCase()) : e
+        kp = function(r) {
+            return eu(r, function(e) {
+                return fp.test(e) ? nu(e.slice(4).toLowerCase()) : e
             })
         },
-        xp = function(r) {
-            return Jc(r, function(e) {
-                return dp.test(e) ? "xn--" + ru(e) : e
+        _p = function(r) {
+            return eu(r, function(e) {
+                return gp.test(e) ? "xn--" + iu(e) : e
             })
         },
-        vp = {
+        Sp = {
             version: "2.3.1",
             ucs2: {
-                decode: Kc,
-                encode: gp
+                decode: tu,
+                encode: vp
             },
-            decode: tu,
-            encode: ru,
-            toASCII: xp,
-            toUnicode: yp
+            decode: nu,
+            encode: iu,
+            toASCII: _p,
+            toUnicode: kp
         };
-    nu.exports = vp
+    ou.exports = Sp
 });
-var au = W((P2, ou) => {
+var lu = W((Y2, su) => {
     "use strict";
-    ou.exports = {
+    su.exports = {
         options: {
             html: !1,
             xhtmlOut: !1,
             breaks: !1,
             langPrefix: "language-",
             linkify: !1,
             typographer: !1,
@@ -5482,17 +5482,17 @@
         components: {
             core: {},
             block: {},
             inline: {}
         }
     }
 });
-var lu = W((I2, su) => {
+var uu = W((Z2, cu) => {
     "use strict";
-    su.exports = {
+    cu.exports = {
         options: {
             html: !1,
             xhtmlOut: !1,
             breaks: !1,
             langPrefix: "language-",
             linkify: !1,
             typographer: !1,
@@ -5510,17 +5510,17 @@
             inline: {
                 rules: ["text"],
                 rules2: ["balance_pairs", "fragments_join"]
             }
         }
     }
 });
-var uu = W((O2, cu) => {
+var du = W((Q2, hu) => {
     "use strict";
-    cu.exports = {
+    hu.exports = {
         options: {
             html: !0,
             xhtmlOut: !0,
             breaks: !1,
             langPrefix: "language-",
             linkify: !1,
             typographer: !1,
@@ -5538,66 +5538,66 @@
             inline: {
                 rules: ["autolink", "backticks", "emphasis", "entity", "escape", "html_inline", "image", "link", "newline", "text"],
                 rules2: ["balance_pairs", "emphasis", "fragments_join"]
             }
         }
     }
 });
-var pu = W((H2, mu) => {
+var gu = W((X2, fu) => {
     "use strict";
     var Ir = Se(),
-        wp = Ys(),
-        kp = Zs(),
-        _p = _l(),
-        Sp = oc(),
-        Cp = $c(),
-        Tp = Qc(),
-        or = ei(),
-        hu = iu(),
-        Ap = {
-            default: au(),
-            zero: lu(),
-            commonmark: uu()
+        Cp = Qs(),
+        Tp = Js(),
+        Ap = Cl(),
+        qp = sc(),
+        Mp = Vc(),
+        Ep = Xc(),
+        ar = ii(),
+        mu = au(),
+        Dp = {
+            default: lu(),
+            zero: uu(),
+            commonmark: du()
         },
-        qp = /^(vbscript|javascript|file|data):/,
-        Mp = /^data:image\/(gif|png|jpeg|webp);/;
+        zp = /^(vbscript|javascript|file|data):/,
+        Rp = /^data:image\/(gif|png|jpeg|webp);/;
 
-    function Ep(r) {
+    function Fp(r) {
         var e = r.trim().toLowerCase();
-        return qp.test(e) ? !!Mp.test(e) : !0
+        return zp.test(e) ? !!Rp.test(e) : !0
     }
-    var du = ["http:", "https:", "mailto:"];
+    var pu = ["http:", "https:", "mailto:"];
 
-    function Dp(r) {
-        var e = or.parse(r, !0);
-        if (e.hostname && (!e.protocol || du.indexOf(e.protocol) >= 0)) try {
-            e.hostname = hu.toASCII(e.hostname)
+    function Bp(r) {
+        var e = ar.parse(r, !0);
+        if (e.hostname && (!e.protocol || pu.indexOf(e.protocol) >= 0)) try {
+            e.hostname = mu.toASCII(e.hostname)
         } catch {}
-        return or.encode(or.format(e))
+        return ar.encode(ar.format(e))
     }
 
-    function zp(r) {
-        var e = or.parse(r, !0);
-        if (e.hostname && (!e.protocol || du.indexOf(e.protocol) >= 0)) try {
-            e.hostname = hu.toUnicode(e.hostname)
+    function Np(r) {
+        var e = ar.parse(r, !0);
+        if (e.hostname && (!e.protocol || pu.indexOf(e.protocol) >= 0)) try {
+            e.hostname = mu.toUnicode(e.hostname)
         } catch {}
-        return or.decode(or.format(e), or.decode.defaultChars + "%")
+        return ar.decode(ar.format(e), ar.decode.defaultChars + "%")
     }
 
     function bt(r, e) {
         if (!(this instanceof bt)) return new bt(r, e);
-        e || Ir.isString(r) || (e = r || {}, r = "default"), this.inline = new Cp, this.block = new Sp, this.core = new _p, this.renderer = new kp, this.linkify = new Tp, this.validateLink = Ep, this.normalizeLink = Dp, this.normalizeLinkText = zp, this.utils = Ir, this.helpers = Ir.assign({}, wp), this.options = {}, this.configure(r), e && this.set(e)
+        e || Ir.isString(r) || (e = r || {}, r = "default"), this.inline = new Mp, this.block = new qp, this.core = new Ap, this.renderer = new Tp, this.linkify = new Ep, this.validateLink = Fp, this.normalizeLink = Bp, this.normalizeLinkText = Np, this.utils = Ir, this.helpers = Ir.assign({}, Cp), this.options = {}, this.configure(r), e && this.set(e)
     }
     bt.prototype.set = function(r) {
         return Ir.assign(this.options, r), this
     };
     bt.prototype.configure = function(r) {
         var e = this,
             i;
-        if (Ir.isString(r) && (i = r, r = Ap[i], !r)) throw new Error('Wrong `markdown-it` preset "' + i + '", check name');
+        if (Ir.isString(r) && (i = r, r = Dp[i], !r)) throw new Error('Wrong `markdown-it` preset "' + i + '", check name');
         if (!r) throw new Error("Wrong `markdown-it` preset, can't be empty");
         return r.options && e.set(r.options), r.components && Object.keys(r.components).forEach(function(a) {
             r.components[a].rules && e[a].ruler.enableOnly(r.components[a].rules), r.components[a].rules2 && e[a].ruler2.enableOnly(r.components[a].rules2)
         }), this
     };
     bt.prototype.enable = function(r, e) {
         var i = [];
@@ -5636,23 +5636,23 @@
     bt.prototype.parseInline = function(r, e) {
         var i = new this.core.State(r, this, e);
         return i.inlineMode = !0, this.core.process(i), i.tokens
     };
     bt.prototype.renderInline = function(r, e) {
         return e = e || {}, this.renderer.render(this.parseInline(r, e), this.options, e)
     };
-    mu.exports = bt
+    fu.exports = bt
 });
-var gu = W(($2, fu) => {
+var yu = W((J2, bu) => {
     "use strict";
-    fu.exports = pu()
+    bu.exports = gu()
 });
-var bu = W((Or, Ci) => {
+var xu = W((Or, Mi) => {
     (function(e, i) {
-        typeof Or == "object" && typeof Ci == "object" ? Ci.exports = i() : typeof define == "function" && define.amd ? define([], i) : typeof Or == "object" ? Or.katex = i() : e.katex = i()
+        typeof Or == "object" && typeof Mi == "object" ? Mi.exports = i() : typeof define == "function" && define.amd ? define([], i) : typeof Or == "object" ? Or.katex = i() : e.katex = i()
     })(typeof self < "u" ? self : Or, function() {
         return function() {
             "use strict";
             var r = {};
             (function() {
                 r.d = function(n, t) {
                     for (var o in t) r.o(t, o) && !r.o(n, o) && Object.defineProperty(n, o, {
@@ -5665,83 +5665,83 @@
                 r.o = function(n, t) {
                     return Object.prototype.hasOwnProperty.call(n, t)
                 }
             }();
             var e = {};
             r.d(e, {
                 default: function() {
-                    return J1
+                    return K1
                 }
             });
             class i {
                 constructor(t, o) {
                     this.name = void 0, this.position = void 0, this.length = void 0, this.rawMessage = void 0;
                     let s = "KaTeX parse error: " + t,
-                        u, f, b = o && o.loc;
+                        u, p, b = o && o.loc;
                     if (b && b.start <= b.end) {
                         let S = b.lexer.input;
-                        u = b.start, f = b.end, u === S.length ? s += " at end of input: " : s += " at position " + (u + 1) + ": ";
-                        let E = S.slice(u, f).replace(/[^]/g, "$&\u0332"),
+                        u = b.start, p = b.end, u === S.length ? s += " at end of input: " : s += " at position " + (u + 1) + ": ";
+                        let E = S.slice(u, p).replace(/[^]/g, "$&\u0332"),
                             z;
                         u > 15 ? z = "\u2026" + S.slice(u - 15, u) : z = S.slice(0, u);
                         let F;
-                        f + 15 < S.length ? F = S.slice(f, f + 15) + "\u2026" : F = S.slice(f), s += z + E + F
+                        p + 15 < S.length ? F = S.slice(p, p + 15) + "\u2026" : F = S.slice(p), s += z + E + F
                     }
                     let v = new Error(s);
-                    return v.name = "ParseError", v.__proto__ = i.prototype, v.position = u, u != null && f != null && (v.length = f - u), v.rawMessage = t, v
+                    return v.name = "ParseError", v.__proto__ = i.prototype, v.position = u, u != null && p != null && (v.length = p - u), v.rawMessage = t, v
                 }
             }
             i.prototype.__proto__ = Error.prototype;
             var a = i;
             let l = function(n, t) {
                     return n.indexOf(t) !== -1
                 },
                 c = function(n, t) {
                     return n === void 0 ? t : n
                 },
                 d = /([A-Z])/g,
-                m = function(n) {
+                f = function(n) {
                     return n.replace(d, "-$1").toLowerCase()
                 },
                 g = {
                     "&": "&amp;",
                     ">": "&gt;",
                     "<": "&lt;",
                     '"': "&quot;",
                     "'": "&#x27;"
                 },
                 y = /[&><"']/g;
 
             function _(n) {
                 return String(n).replace(y, t => g[t])
             }
-            let k = function(n) {
-                    return n.type === "ordgroup" || n.type === "color" ? n.body.length === 1 ? k(n.body[0]) : n : n.type === "font" ? k(n.body) : n
+            let w = function(n) {
+                    return n.type === "ordgroup" || n.type === "color" ? n.body.length === 1 ? w(n.body[0]) : n : n.type === "font" ? w(n.body) : n
                 },
                 T = function(n) {
-                    let t = k(n);
+                    let t = w(n);
                     return t.type === "mathord" || t.type === "textord" || t.type === "atom"
                 },
                 A = function(n) {
                     if (!n) throw new Error("Expected non-null, but got " + String(n));
                     return n
                 };
             var R = {
                 contains: l,
                 deflt: c,
                 escape: _,
-                hyphenate: m,
-                getBaseElem: k,
+                hyphenate: f,
+                getBaseElem: w,
                 isCharacterBox: T,
                 protocolFromUrl: function(n) {
                     let t = /^[\x00-\x20]*([^\\/#?]*?)(:|&#0*58|&#x0*3a|&colon)/i.exec(n);
                     return t ? t[2] !== ":" || !/^[a-zA-Z][a-zA-Z0-9+\-.]*$/.test(t[1]) ? null : t[1].toLowerCase() : "_relative"
                 }
             };
-            let G = {
+            let O = {
                 displayMode: {
                     type: "boolean",
                     description: "Render math in display mode, which puts the math in display style (so \\int and \\sum are large, for example), and centers the math on the page on its own line.",
                     cli: "-d, --display-mode"
                 },
                 output: {
                     type: {
@@ -5840,17 +5840,17 @@
                     case "object":
                         return {}
                 }
             }
             class I {
                 constructor(t) {
                     this.displayMode = void 0, this.output = void 0, this.leqno = void 0, this.fleqn = void 0, this.throwOnError = void 0, this.errorColor = void 0, this.macros = void 0, this.minRuleThickness = void 0, this.colorIsTextColor = void 0, this.strict = void 0, this.trust = void 0, this.maxSize = void 0, this.maxExpand = void 0, this.globalGroup = void 0, t = t || {};
-                    for (let o in G)
-                        if (G.hasOwnProperty(o)) {
-                            let s = G[o];
+                    for (let o in O)
+                        if (O.hasOwnProperty(o)) {
+                            let s = O[o];
                             this[o] = t[o] !== void 0 ? s.processor ? s.processor(t[o]) : t[o] : P(s)
                         }
                 }
                 reportNonstrict(t, o, s) {
                     let u = this.strict;
                     if (typeof u == "function" && (u = u(t, o, s)), !(!u || u === "ignore")) {
                         if (u === !0 || u === "error") throw new a("LaTeX-incompatible input and strict mode is set to 'error': " + (o + " [" + t + "]"), s);
@@ -5912,15 +5912,15 @@
                 De = [new Y(re, 0, !1), new Y(te, 0, !0), new Y(j, 1, !1), new Y(ne, 1, !0), new Y(pe, 2, !1), new Y(ue, 2, !0), new Y(ce, 3, !1), new Y(Ce, 3, !0)],
                 U = [pe, ue, pe, ue, ce, Ce, ce, Ce],
                 X = [ue, ue, ue, ue, Ce, Ce, Ce, Ce],
                 he = [j, ne, pe, ue, ce, Ce, ce, Ce],
                 oe = [ne, ne, ue, ue, Ce, Ce, Ce, Ce],
                 ae = [te, te, ne, ne, ue, ue, Ce, Ce],
                 ee = [re, te, j, ne, j, ne, j, ne];
-            var $ = {
+            var G = {
                 DISPLAY: De[re],
                 TEXT: De[j],
                 SCRIPT: De[pe],
                 SCRIPTSCRIPT: De[ce]
             };
             let fe = [{
                 name: "latin",
@@ -6004,86 +6004,86 @@
 H40000v` + (40 + n) + `H1012.3
 s-271.3,567,-271.3,567c-38.7,80.7,-84,175,-136,283c-52,108,-89.167,185.3,-111.5,232
 c-22.3,46.7,-33.8,70.3,-34.5,71c-4.7,4.7,-12.3,7,-23,7s-12,-1,-12,-1
 s-109,-253,-109,-253c-72.7,-168,-109.3,-252,-110,-252c-10.7,8,-22,16.7,-34,26
 c-22,17.3,-33.3,26,-34,26s-26,-26,-26,-26s76,-59,76,-59s76,-60,76,-60z
 M` + (1001 + n) + " " + t + "h400000v" + (40 + n) + "h-400000z"
                 },
-                O0 = function(n, t) {
+                H0 = function(n, t) {
                     return "M983 " + (10 + n + t) + `
 l` + n / 3.13 + " -" + n + `
 c4,-6.7,10,-10,18,-10 H400000v` + (40 + n) + `
 H1013.1s-83.4,268,-264.1,840c-180.7,572,-277,876.3,-289,913c-4.7,4.7,-12.7,7,-24,7
 s-12,0,-12,0c-1.3,-3.3,-3.7,-11.7,-7,-25c-35.3,-125.3,-106.7,-373.3,-214,-744
 c-10,12,-21,25,-33,39s-32,39,-32,39c-6,-5.3,-15,-14,-27,-26s25,-30,25,-30
 c26.7,-32.7,52,-63,76,-91s52,-60,52,-60s208,722,208,722
 c56,-175.3,126.3,-397.3,211,-666c84.7,-268.7,153.8,-488.2,207.5,-658.5
 c53.7,-170.3,84.5,-266.8,92.5,-289.5z
 M` + (1001 + n) + " " + t + "h400000v" + (40 + n) + "h-400000z"
                 },
-                H0 = function(n, t) {
+                $0 = function(n, t) {
                     return "M424," + (2398 + n + t) + `
 c-1.3,-0.7,-38.5,-172,-111.5,-514c-73,-342,-109.8,-513.3,-110.5,-514
 c0,-2,-10.7,14.3,-32,49c-4.7,7.3,-9.8,15.7,-15.5,25c-5.7,9.3,-9.8,16,-12.5,20
 s-5,7,-5,7c-4,-3.3,-8.3,-7.7,-13,-13s-13,-13,-13,-13s76,-122,76,-122s77,-121,77,-121
 s209,968,209,968c0,-2,84.7,-361.7,254,-1079c169.3,-717.3,254.7,-1077.7,256,-1081
 l` + n / 4.223 + " -" + n + `c4,-6.7,10,-10,18,-10 H400000
 v` + (40 + n) + `H1014.6
 s-87.3,378.7,-272.6,1166c-185.3,787.3,-279.3,1182.3,-282,1185
 c-2,6,-10,9,-24,9
 c-8,0,-12,-0.7,-12,-2z M` + (1001 + n) + " " + t + `
 h400000v` + (40 + n) + "h-400000z"
                 },
-                $0 = function(n, t) {
+                G0 = function(n, t) {
                     return "M473," + (2713 + n + t) + `
 c339.3,-1799.3,509.3,-2700,510,-2702 l` + n / 5.298 + " -" + n + `
 c3.3,-7.3,9.3,-11,18,-11 H400000v` + (40 + n) + `H1017.7
 s-90.5,478,-276.2,1466c-185.7,988,-279.5,1483,-281.5,1485c-2,6,-10,9,-24,9
 c-8,0,-12,-0.7,-12,-2c0,-1.3,-5.3,-32,-16,-92c-50.7,-293.3,-119.7,-693.3,-207,-1200
 c0,-1.3,-5.3,8.7,-16,30c-10.7,21.3,-21.3,42.7,-32,64s-16,33,-16,33s-26,-26,-26,-26
 s76,-153,76,-153s77,-151,77,-151c0.7,0.7,35.7,202,105,604c67.3,400.7,102,602.7,104,
 606zM` + (1001 + n) + " " + t + "h400000v" + (40 + n) + "H1017.7z"
                 },
-                Du = function(n) {
+                zu = function(n) {
                     let t = n / 2;
                     return "M400000 " + n + " H0 L" + t + " 0 l65 45 L145 " + (n - 80) + " H400000z"
                 },
-                zu = function(n, t, o) {
+                Ru = function(n, t, o) {
                     let s = o - 54 - t - n;
                     return "M702 " + (n + t) + "H400000" + (40 + n) + `
 H742v` + s + `l-4 4-4 4c-.667.7 -2 1.5-4 2.5s-4.167 1.833-6.5 2.5-5.5 1-9.5 1
 h-12l-28-84c-16.667-52-96.667 -294.333-240-727l-212 -643 -85 170
 c-4-3.333-8.333-7.667-13 -13l-13-13l77-155 77-156c66 199.333 139 419.667
 219 661 l218 661zM702 ` + t + "H400000v" + (40 + n) + "H742z"
                 },
-                Ru = function(n, t, o) {
+                Fu = function(n, t, o) {
                     t = 1e3 * t;
                     let s = "";
                     switch (n) {
                         case "sqrtMain":
                             s = Pt(t, ct);
                             break;
                         case "sqrtSize1":
                             s = yr(t, ct);
                             break;
                         case "sqrtSize2":
-                            s = O0(t, ct);
+                            s = H0(t, ct);
                             break;
                         case "sqrtSize3":
-                            s = H0(t, ct);
+                            s = $0(t, ct);
                             break;
                         case "sqrtSize4":
-                            s = $0(t, ct);
+                            s = G0(t, ct);
                             break;
                         case "sqrtTall":
-                            s = zu(t, ct, o)
+                            s = Ru(t, ct, o)
                     }
                     return s
                 },
-                Fu = function(n, t) {
+                Bu = function(n, t) {
                     switch (n) {
                         case "\u239C":
                             return "M291 0 H417 V" + t + " H291z M291 0 H417 V" + t + " H291z";
                         case "\u2223":
                             return "M145 0 H188 V" + t + " H145z M145 0 H188 V" + t + " H145z";
                         case "\u2225":
                             return "M145 0 H188 V" + t + " H145z M145 0 H188 V" + t + " H145z" + ("M367 0 H410 V" + t + " H367z M367 0 H410 V" + t + " H367z");
@@ -6099,15 +6099,15 @@
                             return "M312 0 H355 V" + t + " H312z M312 0 H355 V" + t + " H312z";
                         case "\u2016":
                             return "M257 0 H300 V" + t + " H257z M257 0 H300 V" + t + " H257z" + ("M478 0 H521 V" + t + " H478z M478 0 H521 V" + t + " H478z");
                         default:
                             return ""
                     }
                 },
-                Ti = {
+                Ei = {
                     doubleleftarrow: `M262 157
 l10-10c34-36 62.7-77 86-123 3.3-8 5-13.3 5-16 0-5.3-6.7-8-20-8-7.3
  0-12.2.5-14.5 1.5-2.3 1-4.8 4.5-7.5 10.5-49.3 97.3-121.7 169.3-217 216-28
  14-57.3 25-88 33-6.7 2-11 3.8-13 5.5-2 1.7-3 4.2-3 7.5s1 5.8 3 7.5
 c2 1.7 6.3 3.5 13 5.5 68 17.3 128.2 47.8 180.5 91.5 52.3 43.7 93.8 96.2 124.5
  157.5 9.3 8 15.3 12.3 18 13h6c12-.7 18-4 18-10 0-2-1.7-7-5-15-23.3-46-52-87
 -86-123l-10-10h399738v-40H218c328 0 0 0 0 0l-10-8c-26.7-20-65.7-43-117-69 2.7
@@ -6331,15 +6331,15 @@
 M93 435 v40 H400000 v-40z M500 241 v40 H400000 v-40z M500 241 v40 H400000 v-40z`,
                     shortrightharpoonabovebar: `M53,241l0,40c398570,0,399437,0,399437,0
 c4.7,-4.7,7,-9.3,7,-14c0,-9.3,-3.7,-15.3,-11,-18c-92.7,-56.7,-159,-133.7,-199,
 -231c-3.3,-9.3,-6,-14.7,-8,-16c-2,-1.3,-7,-2,-15,-2c-10.7,0,-16.7,2,-18,6
 c-2,2.7,-1,9.7,3,21c15.3,42,36.7,81.8,64,119.5c27.3,37.7,58,69.2,92,94.5z
 M500 241 v40 H399408 v-40z M500 435 v40 H400000 v-40z`
                 },
-                Bu = function(n, t) {
+                Nu = function(n, t) {
                     switch (n) {
                         case "lbrack":
                             return "M403 1759 V84 H666 V0 H319 V1759 v" + t + ` v1759 h347 v-84
 H403z M403 1759 V0 H319 V1759 v` + t + " v1759 h84z";
                         case "rbrack":
                             return "M347 1759 V0 H0 V84 H263 V1759 v" + t + ` v1759 H0 v84 H347z
 M347 1759 V0 H263 V1759 v` + t + " v1759 h84z";
@@ -8483,15 +8483,15 @@
                     937: [0, .61111, 0, 0, .525],
                     8216: [0, .61111, 0, 0, .525],
                     8217: [0, .61111, 0, 0, .525],
                     8242: [0, .61111, 0, 0, .525],
                     9251: [.11111, .21944, 0, 0, .525]
                 }
             };
-            let Hr = {
+            let $r = {
                     slant: [.25, .25, .25],
                     space: [0, 0, 0],
                     stretch: [0, 0, 0],
                     shrink: [0, 0, 0],
                     xHeight: [.431, .431, .431],
                     quad: [1, 1.171, 1.472],
                     extraSpace: [0, 0, 0],
@@ -8519,15 +8519,15 @@
                     sqrtRuleThickness: [.04, .04, .04],
                     ptPerEm: [10, 10, 10],
                     doubleRuleSep: [.2, .2, .2],
                     arrayRuleWidth: [.04, .04, .04],
                     fboxsep: [.3, .3, .3],
                     fboxrule: [.04, .04, .04]
                 },
-                Ai = {
+                Di = {
                     \u00C5: "A",
                     \u00D0: "D",
                     \u00DE: "o",
                     \u00E5: "a",
                     \u00F0: "d",
                     \u00FE: "o",
                     \u0410: "A",
@@ -8592,62 +8592,62 @@
                     \u044B: "m",
                     \u044C: "a",
                     \u044D: "e",
                     \u044E: "m",
                     \u044F: "r"
                 };
 
-            function Nu(n, t) {
+            function Lu(n, t) {
                 vt[n] = t
             }
 
-            function G0(n, t, o) {
+            function V0(n, t, o) {
                 if (!vt[t]) throw new Error("Font metrics not found for font: " + t + ".");
                 let s = n.charCodeAt(0),
                     u = vt[t][s];
-                if (!u && n[0] in Ai && (s = Ai[n[0]].charCodeAt(0), u = vt[t][s]), !u && o === "text" && qt(s) && (u = vt[t][77]), u) return {
+                if (!u && n[0] in Di && (s = Di[n[0]].charCodeAt(0), u = vt[t][s]), !u && o === "text" && qt(s) && (u = vt[t][77]), u) return {
                     depth: u[0],
                     height: u[1],
                     italic: u[2],
                     skew: u[3],
                     width: u[4]
                 }
             }
-            let V0 = {};
+            let j0 = {};
 
-            function Lu(n) {
+            function Pu(n) {
                 let t;
-                if (n >= 5 ? t = 0 : n >= 3 ? t = 1 : t = 2, !V0[t]) {
-                    let o = V0[t] = {
-                        cssEmPerMu: Hr.quad[t] / 18
+                if (n >= 5 ? t = 0 : n >= 3 ? t = 1 : t = 2, !j0[t]) {
+                    let o = j0[t] = {
+                        cssEmPerMu: $r.quad[t] / 18
                     };
-                    for (let s in Hr) Hr.hasOwnProperty(s) && (o[s] = Hr[s][t])
+                    for (let s in $r) $r.hasOwnProperty(s) && (o[s] = $r[s][t])
                 }
-                return V0[t]
+                return j0[t]
             }
-            let Pu = [
+            let Iu = [
                     [1, 1, 1],
                     [2, 1, 1],
                     [3, 1, 1],
                     [4, 2, 1],
                     [5, 2, 1],
                     [6, 3, 1],
                     [7, 4, 2],
                     [8, 6, 3],
                     [9, 7, 6],
                     [10, 8, 7],
                     [11, 10, 9]
                 ],
-                qi = [.5, .6, .7, .8, .9, 1, 1.2, 1.44, 1.728, 2.074, 2.488],
-                Mi = function(n, t) {
-                    return t.size < 2 ? n : Pu[n - 1][t.size - 1]
+                zi = [.5, .6, .7, .8, .9, 1, 1.2, 1.44, 1.728, 2.074, 2.488],
+                Ri = function(n, t) {
+                    return t.size < 2 ? n : Iu[n - 1][t.size - 1]
                 };
             class Mt {
                 constructor(t) {
-                    this.style = void 0, this.color = void 0, this.size = void 0, this.textSize = void 0, this.phantom = void 0, this.font = void 0, this.fontFamily = void 0, this.fontWeight = void 0, this.fontShape = void 0, this.sizeMultiplier = void 0, this.maxSize = void 0, this.minRuleThickness = void 0, this._fontMetrics = void 0, this.style = t.style, this.color = t.color, this.size = t.size || Mt.BASESIZE, this.textSize = t.textSize || this.size, this.phantom = !!t.phantom, this.font = t.font || "", this.fontFamily = t.fontFamily || "", this.fontWeight = t.fontWeight || "", this.fontShape = t.fontShape || "", this.sizeMultiplier = qi[this.size - 1], this.maxSize = t.maxSize, this.minRuleThickness = t.minRuleThickness, this._fontMetrics = void 0
+                    this.style = void 0, this.color = void 0, this.size = void 0, this.textSize = void 0, this.phantom = void 0, this.font = void 0, this.fontFamily = void 0, this.fontWeight = void 0, this.fontShape = void 0, this.sizeMultiplier = void 0, this.maxSize = void 0, this.minRuleThickness = void 0, this._fontMetrics = void 0, this.style = t.style, this.color = t.color, this.size = t.size || Mt.BASESIZE, this.textSize = t.textSize || this.size, this.phantom = !!t.phantom, this.font = t.font || "", this.fontFamily = t.fontFamily || "", this.fontWeight = t.fontWeight || "", this.fontShape = t.fontShape || "", this.sizeMultiplier = zi[this.size - 1], this.maxSize = t.maxSize, this.minRuleThickness = t.minRuleThickness, this._fontMetrics = void 0
                 }
                 extend(t) {
                     let o = {
                         style: this.style,
                         size: this.size,
                         textSize: this.textSize,
                         color: this.color,
@@ -8661,31 +8661,31 @@
                     };
                     for (let s in t) t.hasOwnProperty(s) && (o[s] = t[s]);
                     return new Mt(o)
                 }
                 havingStyle(t) {
                     return this.style === t ? this : this.extend({
                         style: t,
-                        size: Mi(this.textSize, t)
+                        size: Ri(this.textSize, t)
                     })
                 }
                 havingCrampedStyle() {
                     return this.havingStyle(this.style.cramp())
                 }
                 havingSize(t) {
                     return this.size === t && this.textSize === t ? this : this.extend({
                         style: this.style.text(),
                         size: t,
                         textSize: t,
-                        sizeMultiplier: qi[t - 1]
+                        sizeMultiplier: zi[t - 1]
                     })
                 }
                 havingBaseStyle(t) {
                     t = t || this.style.text();
-                    let o = Mi(Mt.BASESIZE, t);
+                    let o = Ri(Mt.BASESIZE, t);
                     return this.size === o && this.textSize === Mt.BASESIZE && this.style === t ? this : this.extend({
                         style: t,
                         size: o
                     })
                 }
                 havingBaseSizing() {
                     let t;
@@ -8742,124 +8742,124 @@
                 sizingClasses(t) {
                     return t.size !== this.size ? ["sizing", "reset-size" + t.size, "size" + this.size] : []
                 }
                 baseSizingClasses() {
                     return this.size !== Mt.BASESIZE ? ["sizing", "reset-size" + this.size, "size" + Mt.BASESIZE] : []
                 }
                 fontMetrics() {
-                    return this._fontMetrics || (this._fontMetrics = Lu(this.size)), this._fontMetrics
+                    return this._fontMetrics || (this._fontMetrics = Pu(this.size)), this._fontMetrics
                 }
                 getColor() {
                     return this.phantom ? "transparent" : this.color
                 }
             }
             Mt.BASESIZE = 6;
-            var Iu = Mt;
-            let j0 = {
+            var Ou = Mt;
+            let U0 = {
                     pt: 1,
                     mm: 7227 / 2540,
                     cm: 7227 / 254,
                     in: 72.27,
                     bp: 803 / 800,
                     pc: 12,
                     dd: 1238 / 1157,
                     cc: 14856 / 1157,
                     nd: 685 / 642,
                     nc: 1370 / 107,
                     sp: 1 / 65536,
                     px: 803 / 800
                 },
-                Ou = {
+                Hu = {
                     ex: !0,
                     em: !0,
                     mu: !0
                 },
-                Ei = function(n) {
-                    return typeof n != "string" && (n = n.unit), n in j0 || n in Ou || n === "ex"
+                Fi = function(n) {
+                    return typeof n != "string" && (n = n.unit), n in U0 || n in Hu || n === "ex"
                 },
                 Ie = function(n, t) {
                     let o;
-                    if (n.unit in j0) o = j0[n.unit] / t.fontMetrics().ptPerEm / t.sizeMultiplier;
+                    if (n.unit in U0) o = U0[n.unit] / t.fontMetrics().ptPerEm / t.sizeMultiplier;
                     else if (n.unit === "mu") o = t.fontMetrics().cssEmPerMu;
                     else {
                         let s;
                         if (t.style.isTight() ? s = t.havingStyle(t.style.text()) : s = t, n.unit === "ex") o = s.fontMetrics().xHeight;
                         else if (n.unit === "em") o = s.fontMetrics().quad;
                         else throw new a("Invalid unit: '" + n.unit + "'");
                         s !== t && (o *= s.sizeMultiplier / t.sizeMultiplier)
                     }
                     return Math.min(n.number * o, t.maxSize)
                 },
-                Q = function(n) {
+                Z = function(n) {
                     return +n.toFixed(4) + "em"
                 },
                 It = function(n) {
                     return n.filter(t => t).join(" ")
                 },
-                Di = function(n, t, o) {
+                Bi = function(n, t, o) {
                     if (this.classes = n || [], this.attributes = {}, this.height = 0, this.depth = 0, this.maxFontSize = 0, this.style = o || {}, t) {
                         t.style.isTight() && this.classes.push("mtight");
                         let s = t.getColor();
                         s && (this.style.color = s)
                     }
                 },
-                zi = function(n) {
+                Ni = function(n) {
                     let t = document.createElement(n);
                     t.className = It(this.classes);
                     for (let o in this.style) this.style.hasOwnProperty(o) && (t.style[o] = this.style[o]);
                     for (let o in this.attributes) this.attributes.hasOwnProperty(o) && t.setAttribute(o, this.attributes[o]);
                     for (let o = 0; o < this.children.length; o++) t.appendChild(this.children[o].toNode());
                     return t
                 },
-                Ri = function(n) {
+                Li = function(n) {
                     let t = "<" + n;
                     this.classes.length && (t += ' class="' + R.escape(It(this.classes)) + '"');
                     let o = "";
                     for (let s in this.style) this.style.hasOwnProperty(s) && (o += R.hyphenate(s) + ":" + this.style[s] + ";");
                     o && (t += ' style="' + R.escape(o) + '"');
                     for (let s in this.attributes) this.attributes.hasOwnProperty(s) && (t += " " + s + '="' + R.escape(this.attributes[s]) + '"');
                     t += ">";
                     for (let s = 0; s < this.children.length; s++) t += this.children[s].toMarkup();
                     return t += "</" + n + ">", t
                 };
             class vr {
                 constructor(t, o, s, u) {
-                    this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.width = void 0, this.maxFontSize = void 0, this.style = void 0, Di.call(this, t, s, u), this.children = o || []
+                    this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.width = void 0, this.maxFontSize = void 0, this.style = void 0, Bi.call(this, t, s, u), this.children = o || []
                 }
                 setAttribute(t, o) {
                     this.attributes[t] = o
                 }
                 hasClass(t) {
                     return R.contains(this.classes, t)
                 }
                 toNode() {
-                    return zi.call(this, "span")
+                    return Ni.call(this, "span")
                 }
                 toMarkup() {
-                    return Ri.call(this, "span")
+                    return Li.call(this, "span")
                 }
             }
-            class U0 {
+            class W0 {
                 constructor(t, o, s, u) {
-                    this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, Di.call(this, o, u), this.children = s || [], this.setAttribute("href", t)
+                    this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, Bi.call(this, o, u), this.children = s || [], this.setAttribute("href", t)
                 }
                 setAttribute(t, o) {
                     this.attributes[t] = o
                 }
                 hasClass(t) {
                     return R.contains(this.classes, t)
                 }
                 toNode() {
-                    return zi.call(this, "a")
+                    return Ni.call(this, "a")
                 }
                 toMarkup() {
-                    return Ri.call(this, "a")
+                    return Li.call(this, "a")
                 }
             }
-            class Hu {
+            class $u {
                 constructor(t, o, s) {
                     this.src = void 0, this.alt = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, this.alt = o, this.src = t, this.classes = ["mord"], this.style = s
                 }
                 hasClass(t) {
                     return R.contains(this.classes, t)
                 }
                 toNode() {
@@ -8871,43 +8871,43 @@
                 toMarkup() {
                     let t = '<img src="' + R.escape(this.src) + '"' + (' alt="' + R.escape(this.alt) + '"'),
                         o = "";
                     for (let s in this.style) this.style.hasOwnProperty(s) && (o += R.hyphenate(s) + ":" + this.style[s] + ";");
                     return o && (t += ' style="' + R.escape(o) + '"'), t += "'/>", t
                 }
             }
-            let $u = {
+            let Gu = {
                 \u00EE: "\u0131\u0302",
                 \u00EF: "\u0131\u0308",
                 \u00ED: "\u0131\u0301",
                 \u00EC: "\u0131\u0300"
             };
             class ut {
-                constructor(t, o, s, u, f, b, v, S) {
-                    this.text = void 0, this.height = void 0, this.depth = void 0, this.italic = void 0, this.skew = void 0, this.width = void 0, this.maxFontSize = void 0, this.classes = void 0, this.style = void 0, this.text = t, this.height = o || 0, this.depth = s || 0, this.italic = u || 0, this.skew = f || 0, this.width = b || 0, this.classes = v || [], this.style = S || {}, this.maxFontSize = 0;
+                constructor(t, o, s, u, p, b, v, S) {
+                    this.text = void 0, this.height = void 0, this.depth = void 0, this.italic = void 0, this.skew = void 0, this.width = void 0, this.maxFontSize = void 0, this.classes = void 0, this.style = void 0, this.text = t, this.height = o || 0, this.depth = s || 0, this.italic = u || 0, this.skew = p || 0, this.width = b || 0, this.classes = v || [], this.style = S || {}, this.maxFontSize = 0;
                     let E = Te(this.text.charCodeAt(0));
-                    E && this.classes.push(E + "_fallback"), /[îïíì]/.test(this.text) && (this.text = $u[this.text])
+                    E && this.classes.push(E + "_fallback"), /[îïíì]/.test(this.text) && (this.text = Gu[this.text])
                 }
                 hasClass(t) {
                     return R.contains(this.classes, t)
                 }
                 toNode() {
                     let t = document.createTextNode(this.text),
                         o = null;
-                    this.italic > 0 && (o = document.createElement("span"), o.style.marginRight = Q(this.italic)), this.classes.length > 0 && (o = o || document.createElement("span"), o.className = It(this.classes));
+                    this.italic > 0 && (o = document.createElement("span"), o.style.marginRight = Z(this.italic)), this.classes.length > 0 && (o = o || document.createElement("span"), o.className = It(this.classes));
                     for (let s in this.style) this.style.hasOwnProperty(s) && (o = o || document.createElement("span"), o.style[s] = this.style[s]);
                     return o ? (o.appendChild(t), o) : t
                 }
                 toMarkup() {
                     let t = !1,
                         o = "<span";
                     this.classes.length && (t = !0, o += ' class="', o += R.escape(It(this.classes)), o += '"');
                     let s = "";
                     this.italic > 0 && (s += "margin-right:" + this.italic + "em;");
-                    for (let f in this.style) this.style.hasOwnProperty(f) && (s += R.hyphenate(f) + ":" + this.style[f] + ";");
+                    for (let p in this.style) this.style.hasOwnProperty(p) && (s += R.hyphenate(p) + ":" + this.style[p] + ";");
                     s && (t = !0, o += ' style="' + R.escape(s) + '"');
                     let u = R.escape(this.text);
                     return t ? (o += ">", o += u, o += "</span>", o) : u
                 }
             }
             class Et {
                 constructor(t, o) {
@@ -8929,21 +8929,21 @@
             }
             class Ot {
                 constructor(t, o) {
                     this.pathName = void 0, this.alternate = void 0, this.pathName = t, this.alternate = o
                 }
                 toNode() {
                     let o = document.createElementNS("http://www.w3.org/2000/svg", "path");
-                    return this.alternate ? o.setAttribute("d", this.alternate) : o.setAttribute("d", Ti[this.pathName]), o
+                    return this.alternate ? o.setAttribute("d", this.alternate) : o.setAttribute("d", Ei[this.pathName]), o
                 }
                 toMarkup() {
-                    return this.alternate ? '<path d="' + R.escape(this.alternate) + '"/>' : '<path d="' + R.escape(Ti[this.pathName]) + '"/>'
+                    return this.alternate ? '<path d="' + R.escape(this.alternate) + '"/>' : '<path d="' + R.escape(Ei[this.pathName]) + '"/>'
                 }
             }
-            class W0 {
+            class Y0 {
                 constructor(t) {
                     this.attributes = void 0, this.attributes = t || {}
                 }
                 toNode() {
                     let o = document.createElementNS("http://www.w3.org/2000/svg", "line");
                     for (let s in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, s) && o.setAttribute(s, this.attributes[s]);
                     return o
@@ -8951,106 +8951,106 @@
                 toMarkup() {
                     let t = "<line";
                     for (let o in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, o) && (t += " " + o + '="' + R.escape(this.attributes[o]) + '"');
                     return t += "/>", t
                 }
             }
 
-            function Fi(n) {
+            function Pi(n) {
                 if (n instanceof ut) return n;
                 throw new Error("Expected symbolNode but got " + String(n) + ".")
             }
 
-            function Gu(n) {
+            function Vu(n) {
                 if (n instanceof vr) return n;
                 throw new Error("Expected span<HtmlDomNode> but got " + String(n) + ".")
             }
-            let Vu = {
+            let ju = {
                     bin: 1,
                     close: 1,
                     inner: 1,
                     open: 1,
                     punct: 1,
                     rel: 1
                 },
-                ju = {
+                Uu = {
                     "accent-token": 1,
                     mathord: 1,
                     "op-token": 1,
                     spacing: 1,
                     textord: 1
                 },
-                $r = {
+                Gr = {
                     math: {},
                     text: {}
                 };
-            var Oe = $r;
+            var Oe = Gr;
 
-            function h(n, t, o, s, u, f) {
-                $r[n][u] = {
+            function h(n, t, o, s, u, p) {
+                Gr[n][u] = {
                     font: t,
                     group: o,
                     replace: s
-                }, f && s && ($r[n][s] = $r[n][u])
+                }, p && s && (Gr[n][s] = Gr[n][u])
             }
-            let p = "math",
-                H = "text",
+            let m = "math",
+                $ = "text",
                 x = "main",
                 C = "ams",
                 Be = "accent-token",
                 J = "bin",
                 et = "close",
-                ar = "inner",
+                sr = "inner",
                 se = "mathord",
                 We = "op-token",
                 at = "open",
-                Gr = "punct",
+                Vr = "punct",
                 q = "rel",
                 Dt = "spacing",
                 D = "textord";
-            h(p, x, q, "\u2261", "\\equiv", !0), h(p, x, q, "\u227A", "\\prec", !0), h(p, x, q, "\u227B", "\\succ", !0), h(p, x, q, "\u223C", "\\sim", !0), h(p, x, q, "\u22A5", "\\perp"), h(p, x, q, "\u2AAF", "\\preceq", !0), h(p, x, q, "\u2AB0", "\\succeq", !0), h(p, x, q, "\u2243", "\\simeq", !0), h(p, x, q, "\u2223", "\\mid", !0), h(p, x, q, "\u226A", "\\ll", !0), h(p, x, q, "\u226B", "\\gg", !0), h(p, x, q, "\u224D", "\\asymp", !0), h(p, x, q, "\u2225", "\\parallel"), h(p, x, q, "\u22C8", "\\bowtie", !0), h(p, x, q, "\u2323", "\\smile", !0), h(p, x, q, "\u2291", "\\sqsubseteq", !0), h(p, x, q, "\u2292", "\\sqsupseteq", !0), h(p, x, q, "\u2250", "\\doteq", !0), h(p, x, q, "\u2322", "\\frown", !0), h(p, x, q, "\u220B", "\\ni", !0), h(p, x, q, "\u221D", "\\propto", !0), h(p, x, q, "\u22A2", "\\vdash", !0), h(p, x, q, "\u22A3", "\\dashv", !0), h(p, x, q, "\u220B", "\\owns"), h(p, x, Gr, ".", "\\ldotp"), h(p, x, Gr, "\u22C5", "\\cdotp"), h(p, x, D, "#", "\\#"), h(H, x, D, "#", "\\#"), h(p, x, D, "&", "\\&"), h(H, x, D, "&", "\\&"), h(p, x, D, "\u2135", "\\aleph", !0), h(p, x, D, "\u2200", "\\forall", !0), h(p, x, D, "\u210F", "\\hbar", !0), h(p, x, D, "\u2203", "\\exists", !0), h(p, x, D, "\u2207", "\\nabla", !0), h(p, x, D, "\u266D", "\\flat", !0), h(p, x, D, "\u2113", "\\ell", !0), h(p, x, D, "\u266E", "\\natural", !0), h(p, x, D, "\u2663", "\\clubsuit", !0), h(p, x, D, "\u2118", "\\wp", !0), h(p, x, D, "\u266F", "\\sharp", !0), h(p, x, D, "\u2662", "\\diamondsuit", !0), h(p, x, D, "\u211C", "\\Re", !0), h(p, x, D, "\u2661", "\\heartsuit", !0), h(p, x, D, "\u2111", "\\Im", !0), h(p, x, D, "\u2660", "\\spadesuit", !0), h(p, x, D, "\xA7", "\\S", !0), h(H, x, D, "\xA7", "\\S"), h(p, x, D, "\xB6", "\\P", !0), h(H, x, D, "\xB6", "\\P"), h(p, x, D, "\u2020", "\\dag"), h(H, x, D, "\u2020", "\\dag"), h(H, x, D, "\u2020", "\\textdagger"), h(p, x, D, "\u2021", "\\ddag"), h(H, x, D, "\u2021", "\\ddag"), h(H, x, D, "\u2021", "\\textdaggerdbl"), h(p, x, et, "\u23B1", "\\rmoustache", !0), h(p, x, at, "\u23B0", "\\lmoustache", !0), h(p, x, et, "\u27EF", "\\rgroup", !0), h(p, x, at, "\u27EE", "\\lgroup", !0), h(p, x, J, "\u2213", "\\mp", !0), h(p, x, J, "\u2296", "\\ominus", !0), h(p, x, J, "\u228E", "\\uplus", !0), h(p, x, J, "\u2293", "\\sqcap", !0), h(p, x, J, "\u2217", "\\ast"), h(p, x, J, "\u2294", "\\sqcup", !0), h(p, x, J, "\u25EF", "\\bigcirc", !0), h(p, x, J, "\u2219", "\\bullet", !0), h(p, x, J, "\u2021", "\\ddagger"), h(p, x, J, "\u2240", "\\wr", !0), h(p, x, J, "\u2A3F", "\\amalg"), h(p, x, J, "&", "\\And"), h(p, x, q, "\u27F5", "\\longleftarrow", !0), h(p, x, q, "\u21D0", "\\Leftarrow", !0), h(p, x, q, "\u27F8", "\\Longleftarrow", !0), h(p, x, q, "\u27F6", "\\longrightarrow", !0), h(p, x, q, "\u21D2", "\\Rightarrow", !0), h(p, x, q, "\u27F9", "\\Longrightarrow", !0), h(p, x, q, "\u2194", "\\leftrightarrow", !0), h(p, x, q, "\u27F7", "\\longleftrightarrow", !0), h(p, x, q, "\u21D4", "\\Leftrightarrow", !0), h(p, x, q, "\u27FA", "\\Longleftrightarrow", !0), h(p, x, q, "\u21A6", "\\mapsto", !0), h(p, x, q, "\u27FC", "\\longmapsto", !0), h(p, x, q, "\u2197", "\\nearrow", !0), h(p, x, q, "\u21A9", "\\hookleftarrow", !0), h(p, x, q, "\u21AA", "\\hookrightarrow", !0), h(p, x, q, "\u2198", "\\searrow", !0), h(p, x, q, "\u21BC", "\\leftharpoonup", !0), h(p, x, q, "\u21C0", "\\rightharpoonup", !0), h(p, x, q, "\u2199", "\\swarrow", !0), h(p, x, q, "\u21BD", "\\leftharpoondown", !0), h(p, x, q, "\u21C1", "\\rightharpoondown", !0), h(p, x, q, "\u2196", "\\nwarrow", !0), h(p, x, q, "\u21CC", "\\rightleftharpoons", !0), h(p, C, q, "\u226E", "\\nless", !0), h(p, C, q, "\uE010", "\\@nleqslant"), h(p, C, q, "\uE011", "\\@nleqq"), h(p, C, q, "\u2A87", "\\lneq", !0), h(p, C, q, "\u2268", "\\lneqq", !0), h(p, C, q, "\uE00C", "\\@lvertneqq"), h(p, C, q, "\u22E6", "\\lnsim", !0), h(p, C, q, "\u2A89", "\\lnapprox", !0), h(p, C, q, "\u2280", "\\nprec", !0), h(p, C, q, "\u22E0", "\\npreceq", !0), h(p, C, q, "\u22E8", "\\precnsim", !0), h(p, C, q, "\u2AB9", "\\precnapprox", !0), h(p, C, q, "\u2241", "\\nsim", !0), h(p, C, q, "\uE006", "\\@nshortmid"), h(p, C, q, "\u2224", "\\nmid", !0), h(p, C, q, "\u22AC", "\\nvdash", !0), h(p, C, q, "\u22AD", "\\nvDash", !0), h(p, C, q, "\u22EA", "\\ntriangleleft"), h(p, C, q, "\u22EC", "\\ntrianglelefteq", !0), h(p, C, q, "\u228A", "\\subsetneq", !0), h(p, C, q, "\uE01A", "\\@varsubsetneq"), h(p, C, q, "\u2ACB", "\\subsetneqq", !0), h(p, C, q, "\uE017", "\\@varsubsetneqq"), h(p, C, q, "\u226F", "\\ngtr", !0), h(p, C, q, "\uE00F", "\\@ngeqslant"), h(p, C, q, "\uE00E", "\\@ngeqq"), h(p, C, q, "\u2A88", "\\gneq", !0), h(p, C, q, "\u2269", "\\gneqq", !0), h(p, C, q, "\uE00D", "\\@gvertneqq"), h(p, C, q, "\u22E7", "\\gnsim", !0), h(p, C, q, "\u2A8A", "\\gnapprox", !0), h(p, C, q, "\u2281", "\\nsucc", !0), h(p, C, q, "\u22E1", "\\nsucceq", !0), h(p, C, q, "\u22E9", "\\succnsim", !0), h(p, C, q, "\u2ABA", "\\succnapprox", !0), h(p, C, q, "\u2246", "\\ncong", !0), h(p, C, q, "\uE007", "\\@nshortparallel"), h(p, C, q, "\u2226", "\\nparallel", !0), h(p, C, q, "\u22AF", "\\nVDash", !0), h(p, C, q, "\u22EB", "\\ntriangleright"), h(p, C, q, "\u22ED", "\\ntrianglerighteq", !0), h(p, C, q, "\uE018", "\\@nsupseteqq"), h(p, C, q, "\u228B", "\\supsetneq", !0), h(p, C, q, "\uE01B", "\\@varsupsetneq"), h(p, C, q, "\u2ACC", "\\supsetneqq", !0), h(p, C, q, "\uE019", "\\@varsupsetneqq"), h(p, C, q, "\u22AE", "\\nVdash", !0), h(p, C, q, "\u2AB5", "\\precneqq", !0), h(p, C, q, "\u2AB6", "\\succneqq", !0), h(p, C, q, "\uE016", "\\@nsubseteqq"), h(p, C, J, "\u22B4", "\\unlhd"), h(p, C, J, "\u22B5", "\\unrhd"), h(p, C, q, "\u219A", "\\nleftarrow", !0), h(p, C, q, "\u219B", "\\nrightarrow", !0), h(p, C, q, "\u21CD", "\\nLeftarrow", !0), h(p, C, q, "\u21CF", "\\nRightarrow", !0), h(p, C, q, "\u21AE", "\\nleftrightarrow", !0), h(p, C, q, "\u21CE", "\\nLeftrightarrow", !0), h(p, C, q, "\u25B3", "\\vartriangle"), h(p, C, D, "\u210F", "\\hslash"), h(p, C, D, "\u25BD", "\\triangledown"), h(p, C, D, "\u25CA", "\\lozenge"), h(p, C, D, "\u24C8", "\\circledS"), h(p, C, D, "\xAE", "\\circledR"), h(H, C, D, "\xAE", "\\circledR"), h(p, C, D, "\u2221", "\\measuredangle", !0), h(p, C, D, "\u2204", "\\nexists"), h(p, C, D, "\u2127", "\\mho"), h(p, C, D, "\u2132", "\\Finv", !0), h(p, C, D, "\u2141", "\\Game", !0), h(p, C, D, "\u2035", "\\backprime"), h(p, C, D, "\u25B2", "\\blacktriangle"), h(p, C, D, "\u25BC", "\\blacktriangledown"), h(p, C, D, "\u25A0", "\\blacksquare"), h(p, C, D, "\u29EB", "\\blacklozenge"), h(p, C, D, "\u2605", "\\bigstar"), h(p, C, D, "\u2222", "\\sphericalangle", !0), h(p, C, D, "\u2201", "\\complement", !0), h(p, C, D, "\xF0", "\\eth", !0), h(H, x, D, "\xF0", "\xF0"), h(p, C, D, "\u2571", "\\diagup"), h(p, C, D, "\u2572", "\\diagdown"), h(p, C, D, "\u25A1", "\\square"), h(p, C, D, "\u25A1", "\\Box"), h(p, C, D, "\u25CA", "\\Diamond"), h(p, C, D, "\xA5", "\\yen", !0), h(H, C, D, "\xA5", "\\yen", !0), h(p, C, D, "\u2713", "\\checkmark", !0), h(H, C, D, "\u2713", "\\checkmark"), h(p, C, D, "\u2136", "\\beth", !0), h(p, C, D, "\u2138", "\\daleth", !0), h(p, C, D, "\u2137", "\\gimel", !0), h(p, C, D, "\u03DD", "\\digamma", !0), h(p, C, D, "\u03F0", "\\varkappa"), h(p, C, at, "\u250C", "\\@ulcorner", !0), h(p, C, et, "\u2510", "\\@urcorner", !0), h(p, C, at, "\u2514", "\\@llcorner", !0), h(p, C, et, "\u2518", "\\@lrcorner", !0), h(p, C, q, "\u2266", "\\leqq", !0), h(p, C, q, "\u2A7D", "\\leqslant", !0), h(p, C, q, "\u2A95", "\\eqslantless", !0), h(p, C, q, "\u2272", "\\lesssim", !0), h(p, C, q, "\u2A85", "\\lessapprox", !0), h(p, C, q, "\u224A", "\\approxeq", !0), h(p, C, J, "\u22D6", "\\lessdot"), h(p, C, q, "\u22D8", "\\lll", !0), h(p, C, q, "\u2276", "\\lessgtr", !0), h(p, C, q, "\u22DA", "\\lesseqgtr", !0), h(p, C, q, "\u2A8B", "\\lesseqqgtr", !0), h(p, C, q, "\u2251", "\\doteqdot"), h(p, C, q, "\u2253", "\\risingdotseq", !0), h(p, C, q, "\u2252", "\\fallingdotseq", !0), h(p, C, q, "\u223D", "\\backsim", !0), h(p, C, q, "\u22CD", "\\backsimeq", !0), h(p, C, q, "\u2AC5", "\\subseteqq", !0), h(p, C, q, "\u22D0", "\\Subset", !0), h(p, C, q, "\u228F", "\\sqsubset", !0), h(p, C, q, "\u227C", "\\preccurlyeq", !0), h(p, C, q, "\u22DE", "\\curlyeqprec", !0), h(p, C, q, "\u227E", "\\precsim", !0), h(p, C, q, "\u2AB7", "\\precapprox", !0), h(p, C, q, "\u22B2", "\\vartriangleleft"), h(p, C, q, "\u22B4", "\\trianglelefteq"), h(p, C, q, "\u22A8", "\\vDash", !0), h(p, C, q, "\u22AA", "\\Vvdash", !0), h(p, C, q, "\u2323", "\\smallsmile"), h(p, C, q, "\u2322", "\\smallfrown"), h(p, C, q, "\u224F", "\\bumpeq", !0), h(p, C, q, "\u224E", "\\Bumpeq", !0), h(p, C, q, "\u2267", "\\geqq", !0), h(p, C, q, "\u2A7E", "\\geqslant", !0), h(p, C, q, "\u2A96", "\\eqslantgtr", !0), h(p, C, q, "\u2273", "\\gtrsim", !0), h(p, C, q, "\u2A86", "\\gtrapprox", !0), h(p, C, J, "\u22D7", "\\gtrdot"), h(p, C, q, "\u22D9", "\\ggg", !0), h(p, C, q, "\u2277", "\\gtrless", !0), h(p, C, q, "\u22DB", "\\gtreqless", !0), h(p, C, q, "\u2A8C", "\\gtreqqless", !0), h(p, C, q, "\u2256", "\\eqcirc", !0), h(p, C, q, "\u2257", "\\circeq", !0), h(p, C, q, "\u225C", "\\triangleq", !0), h(p, C, q, "\u223C", "\\thicksim"), h(p, C, q, "\u2248", "\\thickapprox"), h(p, C, q, "\u2AC6", "\\supseteqq", !0), h(p, C, q, "\u22D1", "\\Supset", !0), h(p, C, q, "\u2290", "\\sqsupset", !0), h(p, C, q, "\u227D", "\\succcurlyeq", !0), h(p, C, q, "\u22DF", "\\curlyeqsucc", !0), h(p, C, q, "\u227F", "\\succsim", !0), h(p, C, q, "\u2AB8", "\\succapprox", !0), h(p, C, q, "\u22B3", "\\vartriangleright"), h(p, C, q, "\u22B5", "\\trianglerighteq"), h(p, C, q, "\u22A9", "\\Vdash", !0), h(p, C, q, "\u2223", "\\shortmid"), h(p, C, q, "\u2225", "\\shortparallel"), h(p, C, q, "\u226C", "\\between", !0), h(p, C, q, "\u22D4", "\\pitchfork", !0), h(p, C, q, "\u221D", "\\varpropto"), h(p, C, q, "\u25C0", "\\blacktriangleleft"), h(p, C, q, "\u2234", "\\therefore", !0), h(p, C, q, "\u220D", "\\backepsilon"), h(p, C, q, "\u25B6", "\\blacktriangleright"), h(p, C, q, "\u2235", "\\because", !0), h(p, C, q, "\u22D8", "\\llless"), h(p, C, q, "\u22D9", "\\gggtr"), h(p, C, J, "\u22B2", "\\lhd"), h(p, C, J, "\u22B3", "\\rhd"), h(p, C, q, "\u2242", "\\eqsim", !0), h(p, x, q, "\u22C8", "\\Join"), h(p, C, q, "\u2251", "\\Doteq", !0), h(p, C, J, "\u2214", "\\dotplus", !0), h(p, C, J, "\u2216", "\\smallsetminus"), h(p, C, J, "\u22D2", "\\Cap", !0), h(p, C, J, "\u22D3", "\\Cup", !0), h(p, C, J, "\u2A5E", "\\doublebarwedge", !0), h(p, C, J, "\u229F", "\\boxminus", !0), h(p, C, J, "\u229E", "\\boxplus", !0), h(p, C, J, "\u22C7", "\\divideontimes", !0), h(p, C, J, "\u22C9", "\\ltimes", !0), h(p, C, J, "\u22CA", "\\rtimes", !0), h(p, C, J, "\u22CB", "\\leftthreetimes", !0), h(p, C, J, "\u22CC", "\\rightthreetimes", !0), h(p, C, J, "\u22CF", "\\curlywedge", !0), h(p, C, J, "\u22CE", "\\curlyvee", !0), h(p, C, J, "\u229D", "\\circleddash", !0), h(p, C, J, "\u229B", "\\circledast", !0), h(p, C, J, "\u22C5", "\\centerdot"), h(p, C, J, "\u22BA", "\\intercal", !0), h(p, C, J, "\u22D2", "\\doublecap"), h(p, C, J, "\u22D3", "\\doublecup"), h(p, C, J, "\u22A0", "\\boxtimes", !0), h(p, C, q, "\u21E2", "\\dashrightarrow", !0), h(p, C, q, "\u21E0", "\\dashleftarrow", !0), h(p, C, q, "\u21C7", "\\leftleftarrows", !0), h(p, C, q, "\u21C6", "\\leftrightarrows", !0), h(p, C, q, "\u21DA", "\\Lleftarrow", !0), h(p, C, q, "\u219E", "\\twoheadleftarrow", !0), h(p, C, q, "\u21A2", "\\leftarrowtail", !0), h(p, C, q, "\u21AB", "\\looparrowleft", !0), h(p, C, q, "\u21CB", "\\leftrightharpoons", !0), h(p, C, q, "\u21B6", "\\curvearrowleft", !0), h(p, C, q, "\u21BA", "\\circlearrowleft", !0), h(p, C, q, "\u21B0", "\\Lsh", !0), h(p, C, q, "\u21C8", "\\upuparrows", !0), h(p, C, q, "\u21BF", "\\upharpoonleft", !0), h(p, C, q, "\u21C3", "\\downharpoonleft", !0), h(p, x, q, "\u22B6", "\\origof", !0), h(p, x, q, "\u22B7", "\\imageof", !0), h(p, C, q, "\u22B8", "\\multimap", !0), h(p, C, q, "\u21AD", "\\leftrightsquigarrow", !0), h(p, C, q, "\u21C9", "\\rightrightarrows", !0), h(p, C, q, "\u21C4", "\\rightleftarrows", !0), h(p, C, q, "\u21A0", "\\twoheadrightarrow", !0), h(p, C, q, "\u21A3", "\\rightarrowtail", !0), h(p, C, q, "\u21AC", "\\looparrowright", !0), h(p, C, q, "\u21B7", "\\curvearrowright", !0), h(p, C, q, "\u21BB", "\\circlearrowright", !0), h(p, C, q, "\u21B1", "\\Rsh", !0), h(p, C, q, "\u21CA", "\\downdownarrows", !0), h(p, C, q, "\u21BE", "\\upharpoonright", !0), h(p, C, q, "\u21C2", "\\downharpoonright", !0), h(p, C, q, "\u21DD", "\\rightsquigarrow", !0), h(p, C, q, "\u21DD", "\\leadsto"), h(p, C, q, "\u21DB", "\\Rrightarrow", !0), h(p, C, q, "\u21BE", "\\restriction"), h(p, x, D, "\u2018", "`"), h(p, x, D, "$", "\\$"), h(H, x, D, "$", "\\$"), h(H, x, D, "$", "\\textdollar"), h(p, x, D, "%", "\\%"), h(H, x, D, "%", "\\%"), h(p, x, D, "_", "\\_"), h(H, x, D, "_", "\\_"), h(H, x, D, "_", "\\textunderscore"), h(p, x, D, "\u2220", "\\angle", !0), h(p, x, D, "\u221E", "\\infty", !0), h(p, x, D, "\u2032", "\\prime"), h(p, x, D, "\u25B3", "\\triangle"), h(p, x, D, "\u0393", "\\Gamma", !0), h(p, x, D, "\u0394", "\\Delta", !0), h(p, x, D, "\u0398", "\\Theta", !0), h(p, x, D, "\u039B", "\\Lambda", !0), h(p, x, D, "\u039E", "\\Xi", !0), h(p, x, D, "\u03A0", "\\Pi", !0), h(p, x, D, "\u03A3", "\\Sigma", !0), h(p, x, D, "\u03A5", "\\Upsilon", !0), h(p, x, D, "\u03A6", "\\Phi", !0), h(p, x, D, "\u03A8", "\\Psi", !0), h(p, x, D, "\u03A9", "\\Omega", !0), h(p, x, D, "A", "\u0391"), h(p, x, D, "B", "\u0392"), h(p, x, D, "E", "\u0395"), h(p, x, D, "Z", "\u0396"), h(p, x, D, "H", "\u0397"), h(p, x, D, "I", "\u0399"), h(p, x, D, "K", "\u039A"), h(p, x, D, "M", "\u039C"), h(p, x, D, "N", "\u039D"), h(p, x, D, "O", "\u039F"), h(p, x, D, "P", "\u03A1"), h(p, x, D, "T", "\u03A4"), h(p, x, D, "X", "\u03A7"), h(p, x, D, "\xAC", "\\neg", !0), h(p, x, D, "\xAC", "\\lnot"), h(p, x, D, "\u22A4", "\\top"), h(p, x, D, "\u22A5", "\\bot"), h(p, x, D, "\u2205", "\\emptyset"), h(p, C, D, "\u2205", "\\varnothing"), h(p, x, se, "\u03B1", "\\alpha", !0), h(p, x, se, "\u03B2", "\\beta", !0), h(p, x, se, "\u03B3", "\\gamma", !0), h(p, x, se, "\u03B4", "\\delta", !0), h(p, x, se, "\u03F5", "\\epsilon", !0), h(p, x, se, "\u03B6", "\\zeta", !0), h(p, x, se, "\u03B7", "\\eta", !0), h(p, x, se, "\u03B8", "\\theta", !0), h(p, x, se, "\u03B9", "\\iota", !0), h(p, x, se, "\u03BA", "\\kappa", !0), h(p, x, se, "\u03BB", "\\lambda", !0), h(p, x, se, "\u03BC", "\\mu", !0), h(p, x, se, "\u03BD", "\\nu", !0), h(p, x, se, "\u03BE", "\\xi", !0), h(p, x, se, "\u03BF", "\\omicron", !0), h(p, x, se, "\u03C0", "\\pi", !0), h(p, x, se, "\u03C1", "\\rho", !0), h(p, x, se, "\u03C3", "\\sigma", !0), h(p, x, se, "\u03C4", "\\tau", !0), h(p, x, se, "\u03C5", "\\upsilon", !0), h(p, x, se, "\u03D5", "\\phi", !0), h(p, x, se, "\u03C7", "\\chi", !0), h(p, x, se, "\u03C8", "\\psi", !0), h(p, x, se, "\u03C9", "\\omega", !0), h(p, x, se, "\u03B5", "\\varepsilon", !0), h(p, x, se, "\u03D1", "\\vartheta", !0), h(p, x, se, "\u03D6", "\\varpi", !0), h(p, x, se, "\u03F1", "\\varrho", !0), h(p, x, se, "\u03C2", "\\varsigma", !0), h(p, x, se, "\u03C6", "\\varphi", !0), h(p, x, J, "\u2217", "*", !0), h(p, x, J, "+", "+"), h(p, x, J, "\u2212", "-", !0), h(p, x, J, "\u22C5", "\\cdot", !0), h(p, x, J, "\u2218", "\\circ", !0), h(p, x, J, "\xF7", "\\div", !0), h(p, x, J, "\xB1", "\\pm", !0), h(p, x, J, "\xD7", "\\times", !0), h(p, x, J, "\u2229", "\\cap", !0), h(p, x, J, "\u222A", "\\cup", !0), h(p, x, J, "\u2216", "\\setminus", !0), h(p, x, J, "\u2227", "\\land"), h(p, x, J, "\u2228", "\\lor"), h(p, x, J, "\u2227", "\\wedge", !0), h(p, x, J, "\u2228", "\\vee", !0), h(p, x, D, "\u221A", "\\surd"), h(p, x, at, "\u27E8", "\\langle", !0), h(p, x, at, "\u2223", "\\lvert"), h(p, x, at, "\u2225", "\\lVert"), h(p, x, et, "?", "?"), h(p, x, et, "!", "!"), h(p, x, et, "\u27E9", "\\rangle", !0), h(p, x, et, "\u2223", "\\rvert"), h(p, x, et, "\u2225", "\\rVert"), h(p, x, q, "=", "="), h(p, x, q, ":", ":"), h(p, x, q, "\u2248", "\\approx", !0), h(p, x, q, "\u2245", "\\cong", !0), h(p, x, q, "\u2265", "\\ge"), h(p, x, q, "\u2265", "\\geq", !0), h(p, x, q, "\u2190", "\\gets"), h(p, x, q, ">", "\\gt", !0), h(p, x, q, "\u2208", "\\in", !0), h(p, x, q, "\uE020", "\\@not"), h(p, x, q, "\u2282", "\\subset", !0), h(p, x, q, "\u2283", "\\supset", !0), h(p, x, q, "\u2286", "\\subseteq", !0), h(p, x, q, "\u2287", "\\supseteq", !0), h(p, C, q, "\u2288", "\\nsubseteq", !0), h(p, C, q, "\u2289", "\\nsupseteq", !0), h(p, x, q, "\u22A8", "\\models"), h(p, x, q, "\u2190", "\\leftarrow", !0), h(p, x, q, "\u2264", "\\le"), h(p, x, q, "\u2264", "\\leq", !0), h(p, x, q, "<", "\\lt", !0), h(p, x, q, "\u2192", "\\rightarrow", !0), h(p, x, q, "\u2192", "\\to"), h(p, C, q, "\u2271", "\\ngeq", !0), h(p, C, q, "\u2270", "\\nleq", !0), h(p, x, Dt, "\xA0", "\\ "), h(p, x, Dt, "\xA0", "\\space"), h(p, x, Dt, "\xA0", "\\nobreakspace"), h(H, x, Dt, "\xA0", "\\ "), h(H, x, Dt, "\xA0", " "), h(H, x, Dt, "\xA0", "\\space"), h(H, x, Dt, "\xA0", "\\nobreakspace"), h(p, x, Dt, null, "\\nobreak"), h(p, x, Dt, null, "\\allowbreak"), h(p, x, Gr, ",", ","), h(p, x, Gr, ";", ";"), h(p, C, J, "\u22BC", "\\barwedge", !0), h(p, C, J, "\u22BB", "\\veebar", !0), h(p, x, J, "\u2299", "\\odot", !0), h(p, x, J, "\u2295", "\\oplus", !0), h(p, x, J, "\u2297", "\\otimes", !0), h(p, x, D, "\u2202", "\\partial", !0), h(p, x, J, "\u2298", "\\oslash", !0), h(p, C, J, "\u229A", "\\circledcirc", !0), h(p, C, J, "\u22A1", "\\boxdot", !0), h(p, x, J, "\u25B3", "\\bigtriangleup"), h(p, x, J, "\u25BD", "\\bigtriangledown"), h(p, x, J, "\u2020", "\\dagger"), h(p, x, J, "\u22C4", "\\diamond"), h(p, x, J, "\u22C6", "\\star"), h(p, x, J, "\u25C3", "\\triangleleft"), h(p, x, J, "\u25B9", "\\triangleright"), h(p, x, at, "{", "\\{"), h(H, x, D, "{", "\\{"), h(H, x, D, "{", "\\textbraceleft"), h(p, x, et, "}", "\\}"), h(H, x, D, "}", "\\}"), h(H, x, D, "}", "\\textbraceright"), h(p, x, at, "{", "\\lbrace"), h(p, x, et, "}", "\\rbrace"), h(p, x, at, "[", "\\lbrack", !0), h(H, x, D, "[", "\\lbrack", !0), h(p, x, et, "]", "\\rbrack", !0), h(H, x, D, "]", "\\rbrack", !0), h(p, x, at, "(", "\\lparen", !0), h(p, x, et, ")", "\\rparen", !0), h(H, x, D, "<", "\\textless", !0), h(H, x, D, ">", "\\textgreater", !0), h(p, x, at, "\u230A", "\\lfloor", !0), h(p, x, et, "\u230B", "\\rfloor", !0), h(p, x, at, "\u2308", "\\lceil", !0), h(p, x, et, "\u2309", "\\rceil", !0), h(p, x, D, "\\", "\\backslash"), h(p, x, D, "\u2223", "|"), h(p, x, D, "\u2223", "\\vert"), h(H, x, D, "|", "\\textbar", !0), h(p, x, D, "\u2225", "\\|"), h(p, x, D, "\u2225", "\\Vert"), h(H, x, D, "\u2225", "\\textbardbl"), h(H, x, D, "~", "\\textasciitilde"), h(H, x, D, "\\", "\\textbackslash"), h(H, x, D, "^", "\\textasciicircum"), h(p, x, q, "\u2191", "\\uparrow", !0), h(p, x, q, "\u21D1", "\\Uparrow", !0), h(p, x, q, "\u2193", "\\downarrow", !0), h(p, x, q, "\u21D3", "\\Downarrow", !0), h(p, x, q, "\u2195", "\\updownarrow", !0), h(p, x, q, "\u21D5", "\\Updownarrow", !0), h(p, x, We, "\u2210", "\\coprod"), h(p, x, We, "\u22C1", "\\bigvee"), h(p, x, We, "\u22C0", "\\bigwedge"), h(p, x, We, "\u2A04", "\\biguplus"), h(p, x, We, "\u22C2", "\\bigcap"), h(p, x, We, "\u22C3", "\\bigcup"), h(p, x, We, "\u222B", "\\int"), h(p, x, We, "\u222B", "\\intop"), h(p, x, We, "\u222C", "\\iint"), h(p, x, We, "\u222D", "\\iiint"), h(p, x, We, "\u220F", "\\prod"), h(p, x, We, "\u2211", "\\sum"), h(p, x, We, "\u2A02", "\\bigotimes"), h(p, x, We, "\u2A01", "\\bigoplus"), h(p, x, We, "\u2A00", "\\bigodot"), h(p, x, We, "\u222E", "\\oint"), h(p, x, We, "\u222F", "\\oiint"), h(p, x, We, "\u2230", "\\oiiint"), h(p, x, We, "\u2A06", "\\bigsqcup"), h(p, x, We, "\u222B", "\\smallint"), h(H, x, ar, "\u2026", "\\textellipsis"), h(p, x, ar, "\u2026", "\\mathellipsis"), h(H, x, ar, "\u2026", "\\ldots", !0), h(p, x, ar, "\u2026", "\\ldots", !0), h(p, x, ar, "\u22EF", "\\@cdots", !0), h(p, x, ar, "\u22F1", "\\ddots", !0), h(p, x, D, "\u22EE", "\\varvdots"), h(p, x, Be, "\u02CA", "\\acute"), h(p, x, Be, "\u02CB", "\\grave"), h(p, x, Be, "\xA8", "\\ddot"), h(p, x, Be, "~", "\\tilde"), h(p, x, Be, "\u02C9", "\\bar"), h(p, x, Be, "\u02D8", "\\breve"), h(p, x, Be, "\u02C7", "\\check"), h(p, x, Be, "^", "\\hat"), h(p, x, Be, "\u20D7", "\\vec"), h(p, x, Be, "\u02D9", "\\dot"), h(p, x, Be, "\u02DA", "\\mathring"), h(p, x, se, "\uE131", "\\@imath"), h(p, x, se, "\uE237", "\\@jmath"), h(p, x, D, "\u0131", "\u0131"), h(p, x, D, "\u0237", "\u0237"), h(H, x, D, "\u0131", "\\i", !0), h(H, x, D, "\u0237", "\\j", !0), h(H, x, D, "\xDF", "\\ss", !0), h(H, x, D, "\xE6", "\\ae", !0), h(H, x, D, "\u0153", "\\oe", !0), h(H, x, D, "\xF8", "\\o", !0), h(H, x, D, "\xC6", "\\AE", !0), h(H, x, D, "\u0152", "\\OE", !0), h(H, x, D, "\xD8", "\\O", !0), h(H, x, Be, "\u02CA", "\\'"), h(H, x, Be, "\u02CB", "\\`"), h(H, x, Be, "\u02C6", "\\^"), h(H, x, Be, "\u02DC", "\\~"), h(H, x, Be, "\u02C9", "\\="), h(H, x, Be, "\u02D8", "\\u"), h(H, x, Be, "\u02D9", "\\."), h(H, x, Be, "\xB8", "\\c"), h(H, x, Be, "\u02DA", "\\r"), h(H, x, Be, "\u02C7", "\\v"), h(H, x, Be, "\xA8", '\\"'), h(H, x, Be, "\u02DD", "\\H"), h(H, x, Be, "\u25EF", "\\textcircled");
-            let Bi = {
+            h(m, x, q, "\u2261", "\\equiv", !0), h(m, x, q, "\u227A", "\\prec", !0), h(m, x, q, "\u227B", "\\succ", !0), h(m, x, q, "\u223C", "\\sim", !0), h(m, x, q, "\u22A5", "\\perp"), h(m, x, q, "\u2AAF", "\\preceq", !0), h(m, x, q, "\u2AB0", "\\succeq", !0), h(m, x, q, "\u2243", "\\simeq", !0), h(m, x, q, "\u2223", "\\mid", !0), h(m, x, q, "\u226A", "\\ll", !0), h(m, x, q, "\u226B", "\\gg", !0), h(m, x, q, "\u224D", "\\asymp", !0), h(m, x, q, "\u2225", "\\parallel"), h(m, x, q, "\u22C8", "\\bowtie", !0), h(m, x, q, "\u2323", "\\smile", !0), h(m, x, q, "\u2291", "\\sqsubseteq", !0), h(m, x, q, "\u2292", "\\sqsupseteq", !0), h(m, x, q, "\u2250", "\\doteq", !0), h(m, x, q, "\u2322", "\\frown", !0), h(m, x, q, "\u220B", "\\ni", !0), h(m, x, q, "\u221D", "\\propto", !0), h(m, x, q, "\u22A2", "\\vdash", !0), h(m, x, q, "\u22A3", "\\dashv", !0), h(m, x, q, "\u220B", "\\owns"), h(m, x, Vr, ".", "\\ldotp"), h(m, x, Vr, "\u22C5", "\\cdotp"), h(m, x, D, "#", "\\#"), h($, x, D, "#", "\\#"), h(m, x, D, "&", "\\&"), h($, x, D, "&", "\\&"), h(m, x, D, "\u2135", "\\aleph", !0), h(m, x, D, "\u2200", "\\forall", !0), h(m, x, D, "\u210F", "\\hbar", !0), h(m, x, D, "\u2203", "\\exists", !0), h(m, x, D, "\u2207", "\\nabla", !0), h(m, x, D, "\u266D", "\\flat", !0), h(m, x, D, "\u2113", "\\ell", !0), h(m, x, D, "\u266E", "\\natural", !0), h(m, x, D, "\u2663", "\\clubsuit", !0), h(m, x, D, "\u2118", "\\wp", !0), h(m, x, D, "\u266F", "\\sharp", !0), h(m, x, D, "\u2662", "\\diamondsuit", !0), h(m, x, D, "\u211C", "\\Re", !0), h(m, x, D, "\u2661", "\\heartsuit", !0), h(m, x, D, "\u2111", "\\Im", !0), h(m, x, D, "\u2660", "\\spadesuit", !0), h(m, x, D, "\xA7", "\\S", !0), h($, x, D, "\xA7", "\\S"), h(m, x, D, "\xB6", "\\P", !0), h($, x, D, "\xB6", "\\P"), h(m, x, D, "\u2020", "\\dag"), h($, x, D, "\u2020", "\\dag"), h($, x, D, "\u2020", "\\textdagger"), h(m, x, D, "\u2021", "\\ddag"), h($, x, D, "\u2021", "\\ddag"), h($, x, D, "\u2021", "\\textdaggerdbl"), h(m, x, et, "\u23B1", "\\rmoustache", !0), h(m, x, at, "\u23B0", "\\lmoustache", !0), h(m, x, et, "\u27EF", "\\rgroup", !0), h(m, x, at, "\u27EE", "\\lgroup", !0), h(m, x, J, "\u2213", "\\mp", !0), h(m, x, J, "\u2296", "\\ominus", !0), h(m, x, J, "\u228E", "\\uplus", !0), h(m, x, J, "\u2293", "\\sqcap", !0), h(m, x, J, "\u2217", "\\ast"), h(m, x, J, "\u2294", "\\sqcup", !0), h(m, x, J, "\u25EF", "\\bigcirc", !0), h(m, x, J, "\u2219", "\\bullet", !0), h(m, x, J, "\u2021", "\\ddagger"), h(m, x, J, "\u2240", "\\wr", !0), h(m, x, J, "\u2A3F", "\\amalg"), h(m, x, J, "&", "\\And"), h(m, x, q, "\u27F5", "\\longleftarrow", !0), h(m, x, q, "\u21D0", "\\Leftarrow", !0), h(m, x, q, "\u27F8", "\\Longleftarrow", !0), h(m, x, q, "\u27F6", "\\longrightarrow", !0), h(m, x, q, "\u21D2", "\\Rightarrow", !0), h(m, x, q, "\u27F9", "\\Longrightarrow", !0), h(m, x, q, "\u2194", "\\leftrightarrow", !0), h(m, x, q, "\u27F7", "\\longleftrightarrow", !0), h(m, x, q, "\u21D4", "\\Leftrightarrow", !0), h(m, x, q, "\u27FA", "\\Longleftrightarrow", !0), h(m, x, q, "\u21A6", "\\mapsto", !0), h(m, x, q, "\u27FC", "\\longmapsto", !0), h(m, x, q, "\u2197", "\\nearrow", !0), h(m, x, q, "\u21A9", "\\hookleftarrow", !0), h(m, x, q, "\u21AA", "\\hookrightarrow", !0), h(m, x, q, "\u2198", "\\searrow", !0), h(m, x, q, "\u21BC", "\\leftharpoonup", !0), h(m, x, q, "\u21C0", "\\rightharpoonup", !0), h(m, x, q, "\u2199", "\\swarrow", !0), h(m, x, q, "\u21BD", "\\leftharpoondown", !0), h(m, x, q, "\u21C1", "\\rightharpoondown", !0), h(m, x, q, "\u2196", "\\nwarrow", !0), h(m, x, q, "\u21CC", "\\rightleftharpoons", !0), h(m, C, q, "\u226E", "\\nless", !0), h(m, C, q, "\uE010", "\\@nleqslant"), h(m, C, q, "\uE011", "\\@nleqq"), h(m, C, q, "\u2A87", "\\lneq", !0), h(m, C, q, "\u2268", "\\lneqq", !0), h(m, C, q, "\uE00C", "\\@lvertneqq"), h(m, C, q, "\u22E6", "\\lnsim", !0), h(m, C, q, "\u2A89", "\\lnapprox", !0), h(m, C, q, "\u2280", "\\nprec", !0), h(m, C, q, "\u22E0", "\\npreceq", !0), h(m, C, q, "\u22E8", "\\precnsim", !0), h(m, C, q, "\u2AB9", "\\precnapprox", !0), h(m, C, q, "\u2241", "\\nsim", !0), h(m, C, q, "\uE006", "\\@nshortmid"), h(m, C, q, "\u2224", "\\nmid", !0), h(m, C, q, "\u22AC", "\\nvdash", !0), h(m, C, q, "\u22AD", "\\nvDash", !0), h(m, C, q, "\u22EA", "\\ntriangleleft"), h(m, C, q, "\u22EC", "\\ntrianglelefteq", !0), h(m, C, q, "\u228A", "\\subsetneq", !0), h(m, C, q, "\uE01A", "\\@varsubsetneq"), h(m, C, q, "\u2ACB", "\\subsetneqq", !0), h(m, C, q, "\uE017", "\\@varsubsetneqq"), h(m, C, q, "\u226F", "\\ngtr", !0), h(m, C, q, "\uE00F", "\\@ngeqslant"), h(m, C, q, "\uE00E", "\\@ngeqq"), h(m, C, q, "\u2A88", "\\gneq", !0), h(m, C, q, "\u2269", "\\gneqq", !0), h(m, C, q, "\uE00D", "\\@gvertneqq"), h(m, C, q, "\u22E7", "\\gnsim", !0), h(m, C, q, "\u2A8A", "\\gnapprox", !0), h(m, C, q, "\u2281", "\\nsucc", !0), h(m, C, q, "\u22E1", "\\nsucceq", !0), h(m, C, q, "\u22E9", "\\succnsim", !0), h(m, C, q, "\u2ABA", "\\succnapprox", !0), h(m, C, q, "\u2246", "\\ncong", !0), h(m, C, q, "\uE007", "\\@nshortparallel"), h(m, C, q, "\u2226", "\\nparallel", !0), h(m, C, q, "\u22AF", "\\nVDash", !0), h(m, C, q, "\u22EB", "\\ntriangleright"), h(m, C, q, "\u22ED", "\\ntrianglerighteq", !0), h(m, C, q, "\uE018", "\\@nsupseteqq"), h(m, C, q, "\u228B", "\\supsetneq", !0), h(m, C, q, "\uE01B", "\\@varsupsetneq"), h(m, C, q, "\u2ACC", "\\supsetneqq", !0), h(m, C, q, "\uE019", "\\@varsupsetneqq"), h(m, C, q, "\u22AE", "\\nVdash", !0), h(m, C, q, "\u2AB5", "\\precneqq", !0), h(m, C, q, "\u2AB6", "\\succneqq", !0), h(m, C, q, "\uE016", "\\@nsubseteqq"), h(m, C, J, "\u22B4", "\\unlhd"), h(m, C, J, "\u22B5", "\\unrhd"), h(m, C, q, "\u219A", "\\nleftarrow", !0), h(m, C, q, "\u219B", "\\nrightarrow", !0), h(m, C, q, "\u21CD", "\\nLeftarrow", !0), h(m, C, q, "\u21CF", "\\nRightarrow", !0), h(m, C, q, "\u21AE", "\\nleftrightarrow", !0), h(m, C, q, "\u21CE", "\\nLeftrightarrow", !0), h(m, C, q, "\u25B3", "\\vartriangle"), h(m, C, D, "\u210F", "\\hslash"), h(m, C, D, "\u25BD", "\\triangledown"), h(m, C, D, "\u25CA", "\\lozenge"), h(m, C, D, "\u24C8", "\\circledS"), h(m, C, D, "\xAE", "\\circledR"), h($, C, D, "\xAE", "\\circledR"), h(m, C, D, "\u2221", "\\measuredangle", !0), h(m, C, D, "\u2204", "\\nexists"), h(m, C, D, "\u2127", "\\mho"), h(m, C, D, "\u2132", "\\Finv", !0), h(m, C, D, "\u2141", "\\Game", !0), h(m, C, D, "\u2035", "\\backprime"), h(m, C, D, "\u25B2", "\\blacktriangle"), h(m, C, D, "\u25BC", "\\blacktriangledown"), h(m, C, D, "\u25A0", "\\blacksquare"), h(m, C, D, "\u29EB", "\\blacklozenge"), h(m, C, D, "\u2605", "\\bigstar"), h(m, C, D, "\u2222", "\\sphericalangle", !0), h(m, C, D, "\u2201", "\\complement", !0), h(m, C, D, "\xF0", "\\eth", !0), h($, x, D, "\xF0", "\xF0"), h(m, C, D, "\u2571", "\\diagup"), h(m, C, D, "\u2572", "\\diagdown"), h(m, C, D, "\u25A1", "\\square"), h(m, C, D, "\u25A1", "\\Box"), h(m, C, D, "\u25CA", "\\Diamond"), h(m, C, D, "\xA5", "\\yen", !0), h($, C, D, "\xA5", "\\yen", !0), h(m, C, D, "\u2713", "\\checkmark", !0), h($, C, D, "\u2713", "\\checkmark"), h(m, C, D, "\u2136", "\\beth", !0), h(m, C, D, "\u2138", "\\daleth", !0), h(m, C, D, "\u2137", "\\gimel", !0), h(m, C, D, "\u03DD", "\\digamma", !0), h(m, C, D, "\u03F0", "\\varkappa"), h(m, C, at, "\u250C", "\\@ulcorner", !0), h(m, C, et, "\u2510", "\\@urcorner", !0), h(m, C, at, "\u2514", "\\@llcorner", !0), h(m, C, et, "\u2518", "\\@lrcorner", !0), h(m, C, q, "\u2266", "\\leqq", !0), h(m, C, q, "\u2A7D", "\\leqslant", !0), h(m, C, q, "\u2A95", "\\eqslantless", !0), h(m, C, q, "\u2272", "\\lesssim", !0), h(m, C, q, "\u2A85", "\\lessapprox", !0), h(m, C, q, "\u224A", "\\approxeq", !0), h(m, C, J, "\u22D6", "\\lessdot"), h(m, C, q, "\u22D8", "\\lll", !0), h(m, C, q, "\u2276", "\\lessgtr", !0), h(m, C, q, "\u22DA", "\\lesseqgtr", !0), h(m, C, q, "\u2A8B", "\\lesseqqgtr", !0), h(m, C, q, "\u2251", "\\doteqdot"), h(m, C, q, "\u2253", "\\risingdotseq", !0), h(m, C, q, "\u2252", "\\fallingdotseq", !0), h(m, C, q, "\u223D", "\\backsim", !0), h(m, C, q, "\u22CD", "\\backsimeq", !0), h(m, C, q, "\u2AC5", "\\subseteqq", !0), h(m, C, q, "\u22D0", "\\Subset", !0), h(m, C, q, "\u228F", "\\sqsubset", !0), h(m, C, q, "\u227C", "\\preccurlyeq", !0), h(m, C, q, "\u22DE", "\\curlyeqprec", !0), h(m, C, q, "\u227E", "\\precsim", !0), h(m, C, q, "\u2AB7", "\\precapprox", !0), h(m, C, q, "\u22B2", "\\vartriangleleft"), h(m, C, q, "\u22B4", "\\trianglelefteq"), h(m, C, q, "\u22A8", "\\vDash", !0), h(m, C, q, "\u22AA", "\\Vvdash", !0), h(m, C, q, "\u2323", "\\smallsmile"), h(m, C, q, "\u2322", "\\smallfrown"), h(m, C, q, "\u224F", "\\bumpeq", !0), h(m, C, q, "\u224E", "\\Bumpeq", !0), h(m, C, q, "\u2267", "\\geqq", !0), h(m, C, q, "\u2A7E", "\\geqslant", !0), h(m, C, q, "\u2A96", "\\eqslantgtr", !0), h(m, C, q, "\u2273", "\\gtrsim", !0), h(m, C, q, "\u2A86", "\\gtrapprox", !0), h(m, C, J, "\u22D7", "\\gtrdot"), h(m, C, q, "\u22D9", "\\ggg", !0), h(m, C, q, "\u2277", "\\gtrless", !0), h(m, C, q, "\u22DB", "\\gtreqless", !0), h(m, C, q, "\u2A8C", "\\gtreqqless", !0), h(m, C, q, "\u2256", "\\eqcirc", !0), h(m, C, q, "\u2257", "\\circeq", !0), h(m, C, q, "\u225C", "\\triangleq", !0), h(m, C, q, "\u223C", "\\thicksim"), h(m, C, q, "\u2248", "\\thickapprox"), h(m, C, q, "\u2AC6", "\\supseteqq", !0), h(m, C, q, "\u22D1", "\\Supset", !0), h(m, C, q, "\u2290", "\\sqsupset", !0), h(m, C, q, "\u227D", "\\succcurlyeq", !0), h(m, C, q, "\u22DF", "\\curlyeqsucc", !0), h(m, C, q, "\u227F", "\\succsim", !0), h(m, C, q, "\u2AB8", "\\succapprox", !0), h(m, C, q, "\u22B3", "\\vartriangleright"), h(m, C, q, "\u22B5", "\\trianglerighteq"), h(m, C, q, "\u22A9", "\\Vdash", !0), h(m, C, q, "\u2223", "\\shortmid"), h(m, C, q, "\u2225", "\\shortparallel"), h(m, C, q, "\u226C", "\\between", !0), h(m, C, q, "\u22D4", "\\pitchfork", !0), h(m, C, q, "\u221D", "\\varpropto"), h(m, C, q, "\u25C0", "\\blacktriangleleft"), h(m, C, q, "\u2234", "\\therefore", !0), h(m, C, q, "\u220D", "\\backepsilon"), h(m, C, q, "\u25B6", "\\blacktriangleright"), h(m, C, q, "\u2235", "\\because", !0), h(m, C, q, "\u22D8", "\\llless"), h(m, C, q, "\u22D9", "\\gggtr"), h(m, C, J, "\u22B2", "\\lhd"), h(m, C, J, "\u22B3", "\\rhd"), h(m, C, q, "\u2242", "\\eqsim", !0), h(m, x, q, "\u22C8", "\\Join"), h(m, C, q, "\u2251", "\\Doteq", !0), h(m, C, J, "\u2214", "\\dotplus", !0), h(m, C, J, "\u2216", "\\smallsetminus"), h(m, C, J, "\u22D2", "\\Cap", !0), h(m, C, J, "\u22D3", "\\Cup", !0), h(m, C, J, "\u2A5E", "\\doublebarwedge", !0), h(m, C, J, "\u229F", "\\boxminus", !0), h(m, C, J, "\u229E", "\\boxplus", !0), h(m, C, J, "\u22C7", "\\divideontimes", !0), h(m, C, J, "\u22C9", "\\ltimes", !0), h(m, C, J, "\u22CA", "\\rtimes", !0), h(m, C, J, "\u22CB", "\\leftthreetimes", !0), h(m, C, J, "\u22CC", "\\rightthreetimes", !0), h(m, C, J, "\u22CF", "\\curlywedge", !0), h(m, C, J, "\u22CE", "\\curlyvee", !0), h(m, C, J, "\u229D", "\\circleddash", !0), h(m, C, J, "\u229B", "\\circledast", !0), h(m, C, J, "\u22C5", "\\centerdot"), h(m, C, J, "\u22BA", "\\intercal", !0), h(m, C, J, "\u22D2", "\\doublecap"), h(m, C, J, "\u22D3", "\\doublecup"), h(m, C, J, "\u22A0", "\\boxtimes", !0), h(m, C, q, "\u21E2", "\\dashrightarrow", !0), h(m, C, q, "\u21E0", "\\dashleftarrow", !0), h(m, C, q, "\u21C7", "\\leftleftarrows", !0), h(m, C, q, "\u21C6", "\\leftrightarrows", !0), h(m, C, q, "\u21DA", "\\Lleftarrow", !0), h(m, C, q, "\u219E", "\\twoheadleftarrow", !0), h(m, C, q, "\u21A2", "\\leftarrowtail", !0), h(m, C, q, "\u21AB", "\\looparrowleft", !0), h(m, C, q, "\u21CB", "\\leftrightharpoons", !0), h(m, C, q, "\u21B6", "\\curvearrowleft", !0), h(m, C, q, "\u21BA", "\\circlearrowleft", !0), h(m, C, q, "\u21B0", "\\Lsh", !0), h(m, C, q, "\u21C8", "\\upuparrows", !0), h(m, C, q, "\u21BF", "\\upharpoonleft", !0), h(m, C, q, "\u21C3", "\\downharpoonleft", !0), h(m, x, q, "\u22B6", "\\origof", !0), h(m, x, q, "\u22B7", "\\imageof", !0), h(m, C, q, "\u22B8", "\\multimap", !0), h(m, C, q, "\u21AD", "\\leftrightsquigarrow", !0), h(m, C, q, "\u21C9", "\\rightrightarrows", !0), h(m, C, q, "\u21C4", "\\rightleftarrows", !0), h(m, C, q, "\u21A0", "\\twoheadrightarrow", !0), h(m, C, q, "\u21A3", "\\rightarrowtail", !0), h(m, C, q, "\u21AC", "\\looparrowright", !0), h(m, C, q, "\u21B7", "\\curvearrowright", !0), h(m, C, q, "\u21BB", "\\circlearrowright", !0), h(m, C, q, "\u21B1", "\\Rsh", !0), h(m, C, q, "\u21CA", "\\downdownarrows", !0), h(m, C, q, "\u21BE", "\\upharpoonright", !0), h(m, C, q, "\u21C2", "\\downharpoonright", !0), h(m, C, q, "\u21DD", "\\rightsquigarrow", !0), h(m, C, q, "\u21DD", "\\leadsto"), h(m, C, q, "\u21DB", "\\Rrightarrow", !0), h(m, C, q, "\u21BE", "\\restriction"), h(m, x, D, "\u2018", "`"), h(m, x, D, "$", "\\$"), h($, x, D, "$", "\\$"), h($, x, D, "$", "\\textdollar"), h(m, x, D, "%", "\\%"), h($, x, D, "%", "\\%"), h(m, x, D, "_", "\\_"), h($, x, D, "_", "\\_"), h($, x, D, "_", "\\textunderscore"), h(m, x, D, "\u2220", "\\angle", !0), h(m, x, D, "\u221E", "\\infty", !0), h(m, x, D, "\u2032", "\\prime"), h(m, x, D, "\u25B3", "\\triangle"), h(m, x, D, "\u0393", "\\Gamma", !0), h(m, x, D, "\u0394", "\\Delta", !0), h(m, x, D, "\u0398", "\\Theta", !0), h(m, x, D, "\u039B", "\\Lambda", !0), h(m, x, D, "\u039E", "\\Xi", !0), h(m, x, D, "\u03A0", "\\Pi", !0), h(m, x, D, "\u03A3", "\\Sigma", !0), h(m, x, D, "\u03A5", "\\Upsilon", !0), h(m, x, D, "\u03A6", "\\Phi", !0), h(m, x, D, "\u03A8", "\\Psi", !0), h(m, x, D, "\u03A9", "\\Omega", !0), h(m, x, D, "A", "\u0391"), h(m, x, D, "B", "\u0392"), h(m, x, D, "E", "\u0395"), h(m, x, D, "Z", "\u0396"), h(m, x, D, "H", "\u0397"), h(m, x, D, "I", "\u0399"), h(m, x, D, "K", "\u039A"), h(m, x, D, "M", "\u039C"), h(m, x, D, "N", "\u039D"), h(m, x, D, "O", "\u039F"), h(m, x, D, "P", "\u03A1"), h(m, x, D, "T", "\u03A4"), h(m, x, D, "X", "\u03A7"), h(m, x, D, "\xAC", "\\neg", !0), h(m, x, D, "\xAC", "\\lnot"), h(m, x, D, "\u22A4", "\\top"), h(m, x, D, "\u22A5", "\\bot"), h(m, x, D, "\u2205", "\\emptyset"), h(m, C, D, "\u2205", "\\varnothing"), h(m, x, se, "\u03B1", "\\alpha", !0), h(m, x, se, "\u03B2", "\\beta", !0), h(m, x, se, "\u03B3", "\\gamma", !0), h(m, x, se, "\u03B4", "\\delta", !0), h(m, x, se, "\u03F5", "\\epsilon", !0), h(m, x, se, "\u03B6", "\\zeta", !0), h(m, x, se, "\u03B7", "\\eta", !0), h(m, x, se, "\u03B8", "\\theta", !0), h(m, x, se, "\u03B9", "\\iota", !0), h(m, x, se, "\u03BA", "\\kappa", !0), h(m, x, se, "\u03BB", "\\lambda", !0), h(m, x, se, "\u03BC", "\\mu", !0), h(m, x, se, "\u03BD", "\\nu", !0), h(m, x, se, "\u03BE", "\\xi", !0), h(m, x, se, "\u03BF", "\\omicron", !0), h(m, x, se, "\u03C0", "\\pi", !0), h(m, x, se, "\u03C1", "\\rho", !0), h(m, x, se, "\u03C3", "\\sigma", !0), h(m, x, se, "\u03C4", "\\tau", !0), h(m, x, se, "\u03C5", "\\upsilon", !0), h(m, x, se, "\u03D5", "\\phi", !0), h(m, x, se, "\u03C7", "\\chi", !0), h(m, x, se, "\u03C8", "\\psi", !0), h(m, x, se, "\u03C9", "\\omega", !0), h(m, x, se, "\u03B5", "\\varepsilon", !0), h(m, x, se, "\u03D1", "\\vartheta", !0), h(m, x, se, "\u03D6", "\\varpi", !0), h(m, x, se, "\u03F1", "\\varrho", !0), h(m, x, se, "\u03C2", "\\varsigma", !0), h(m, x, se, "\u03C6", "\\varphi", !0), h(m, x, J, "\u2217", "*", !0), h(m, x, J, "+", "+"), h(m, x, J, "\u2212", "-", !0), h(m, x, J, "\u22C5", "\\cdot", !0), h(m, x, J, "\u2218", "\\circ", !0), h(m, x, J, "\xF7", "\\div", !0), h(m, x, J, "\xB1", "\\pm", !0), h(m, x, J, "\xD7", "\\times", !0), h(m, x, J, "\u2229", "\\cap", !0), h(m, x, J, "\u222A", "\\cup", !0), h(m, x, J, "\u2216", "\\setminus", !0), h(m, x, J, "\u2227", "\\land"), h(m, x, J, "\u2228", "\\lor"), h(m, x, J, "\u2227", "\\wedge", !0), h(m, x, J, "\u2228", "\\vee", !0), h(m, x, D, "\u221A", "\\surd"), h(m, x, at, "\u27E8", "\\langle", !0), h(m, x, at, "\u2223", "\\lvert"), h(m, x, at, "\u2225", "\\lVert"), h(m, x, et, "?", "?"), h(m, x, et, "!", "!"), h(m, x, et, "\u27E9", "\\rangle", !0), h(m, x, et, "\u2223", "\\rvert"), h(m, x, et, "\u2225", "\\rVert"), h(m, x, q, "=", "="), h(m, x, q, ":", ":"), h(m, x, q, "\u2248", "\\approx", !0), h(m, x, q, "\u2245", "\\cong", !0), h(m, x, q, "\u2265", "\\ge"), h(m, x, q, "\u2265", "\\geq", !0), h(m, x, q, "\u2190", "\\gets"), h(m, x, q, ">", "\\gt", !0), h(m, x, q, "\u2208", "\\in", !0), h(m, x, q, "\uE020", "\\@not"), h(m, x, q, "\u2282", "\\subset", !0), h(m, x, q, "\u2283", "\\supset", !0), h(m, x, q, "\u2286", "\\subseteq", !0), h(m, x, q, "\u2287", "\\supseteq", !0), h(m, C, q, "\u2288", "\\nsubseteq", !0), h(m, C, q, "\u2289", "\\nsupseteq", !0), h(m, x, q, "\u22A8", "\\models"), h(m, x, q, "\u2190", "\\leftarrow", !0), h(m, x, q, "\u2264", "\\le"), h(m, x, q, "\u2264", "\\leq", !0), h(m, x, q, "<", "\\lt", !0), h(m, x, q, "\u2192", "\\rightarrow", !0), h(m, x, q, "\u2192", "\\to"), h(m, C, q, "\u2271", "\\ngeq", !0), h(m, C, q, "\u2270", "\\nleq", !0), h(m, x, Dt, "\xA0", "\\ "), h(m, x, Dt, "\xA0", "\\space"), h(m, x, Dt, "\xA0", "\\nobreakspace"), h($, x, Dt, "\xA0", "\\ "), h($, x, Dt, "\xA0", " "), h($, x, Dt, "\xA0", "\\space"), h($, x, Dt, "\xA0", "\\nobreakspace"), h(m, x, Dt, null, "\\nobreak"), h(m, x, Dt, null, "\\allowbreak"), h(m, x, Vr, ",", ","), h(m, x, Vr, ";", ";"), h(m, C, J, "\u22BC", "\\barwedge", !0), h(m, C, J, "\u22BB", "\\veebar", !0), h(m, x, J, "\u2299", "\\odot", !0), h(m, x, J, "\u2295", "\\oplus", !0), h(m, x, J, "\u2297", "\\otimes", !0), h(m, x, D, "\u2202", "\\partial", !0), h(m, x, J, "\u2298", "\\oslash", !0), h(m, C, J, "\u229A", "\\circledcirc", !0), h(m, C, J, "\u22A1", "\\boxdot", !0), h(m, x, J, "\u25B3", "\\bigtriangleup"), h(m, x, J, "\u25BD", "\\bigtriangledown"), h(m, x, J, "\u2020", "\\dagger"), h(m, x, J, "\u22C4", "\\diamond"), h(m, x, J, "\u22C6", "\\star"), h(m, x, J, "\u25C3", "\\triangleleft"), h(m, x, J, "\u25B9", "\\triangleright"), h(m, x, at, "{", "\\{"), h($, x, D, "{", "\\{"), h($, x, D, "{", "\\textbraceleft"), h(m, x, et, "}", "\\}"), h($, x, D, "}", "\\}"), h($, x, D, "}", "\\textbraceright"), h(m, x, at, "{", "\\lbrace"), h(m, x, et, "}", "\\rbrace"), h(m, x, at, "[", "\\lbrack", !0), h($, x, D, "[", "\\lbrack", !0), h(m, x, et, "]", "\\rbrack", !0), h($, x, D, "]", "\\rbrack", !0), h(m, x, at, "(", "\\lparen", !0), h(m, x, et, ")", "\\rparen", !0), h($, x, D, "<", "\\textless", !0), h($, x, D, ">", "\\textgreater", !0), h(m, x, at, "\u230A", "\\lfloor", !0), h(m, x, et, "\u230B", "\\rfloor", !0), h(m, x, at, "\u2308", "\\lceil", !0), h(m, x, et, "\u2309", "\\rceil", !0), h(m, x, D, "\\", "\\backslash"), h(m, x, D, "\u2223", "|"), h(m, x, D, "\u2223", "\\vert"), h($, x, D, "|", "\\textbar", !0), h(m, x, D, "\u2225", "\\|"), h(m, x, D, "\u2225", "\\Vert"), h($, x, D, "\u2225", "\\textbardbl"), h($, x, D, "~", "\\textasciitilde"), h($, x, D, "\\", "\\textbackslash"), h($, x, D, "^", "\\textasciicircum"), h(m, x, q, "\u2191", "\\uparrow", !0), h(m, x, q, "\u21D1", "\\Uparrow", !0), h(m, x, q, "\u2193", "\\downarrow", !0), h(m, x, q, "\u21D3", "\\Downarrow", !0), h(m, x, q, "\u2195", "\\updownarrow", !0), h(m, x, q, "\u21D5", "\\Updownarrow", !0), h(m, x, We, "\u2210", "\\coprod"), h(m, x, We, "\u22C1", "\\bigvee"), h(m, x, We, "\u22C0", "\\bigwedge"), h(m, x, We, "\u2A04", "\\biguplus"), h(m, x, We, "\u22C2", "\\bigcap"), h(m, x, We, "\u22C3", "\\bigcup"), h(m, x, We, "\u222B", "\\int"), h(m, x, We, "\u222B", "\\intop"), h(m, x, We, "\u222C", "\\iint"), h(m, x, We, "\u222D", "\\iiint"), h(m, x, We, "\u220F", "\\prod"), h(m, x, We, "\u2211", "\\sum"), h(m, x, We, "\u2A02", "\\bigotimes"), h(m, x, We, "\u2A01", "\\bigoplus"), h(m, x, We, "\u2A00", "\\bigodot"), h(m, x, We, "\u222E", "\\oint"), h(m, x, We, "\u222F", "\\oiint"), h(m, x, We, "\u2230", "\\oiiint"), h(m, x, We, "\u2A06", "\\bigsqcup"), h(m, x, We, "\u222B", "\\smallint"), h($, x, sr, "\u2026", "\\textellipsis"), h(m, x, sr, "\u2026", "\\mathellipsis"), h($, x, sr, "\u2026", "\\ldots", !0), h(m, x, sr, "\u2026", "\\ldots", !0), h(m, x, sr, "\u22EF", "\\@cdots", !0), h(m, x, sr, "\u22F1", "\\ddots", !0), h(m, x, D, "\u22EE", "\\varvdots"), h(m, x, Be, "\u02CA", "\\acute"), h(m, x, Be, "\u02CB", "\\grave"), h(m, x, Be, "\xA8", "\\ddot"), h(m, x, Be, "~", "\\tilde"), h(m, x, Be, "\u02C9", "\\bar"), h(m, x, Be, "\u02D8", "\\breve"), h(m, x, Be, "\u02C7", "\\check"), h(m, x, Be, "^", "\\hat"), h(m, x, Be, "\u20D7", "\\vec"), h(m, x, Be, "\u02D9", "\\dot"), h(m, x, Be, "\u02DA", "\\mathring"), h(m, x, se, "\uE131", "\\@imath"), h(m, x, se, "\uE237", "\\@jmath"), h(m, x, D, "\u0131", "\u0131"), h(m, x, D, "\u0237", "\u0237"), h($, x, D, "\u0131", "\\i", !0), h($, x, D, "\u0237", "\\j", !0), h($, x, D, "\xDF", "\\ss", !0), h($, x, D, "\xE6", "\\ae", !0), h($, x, D, "\u0153", "\\oe", !0), h($, x, D, "\xF8", "\\o", !0), h($, x, D, "\xC6", "\\AE", !0), h($, x, D, "\u0152", "\\OE", !0), h($, x, D, "\xD8", "\\O", !0), h($, x, Be, "\u02CA", "\\'"), h($, x, Be, "\u02CB", "\\`"), h($, x, Be, "\u02C6", "\\^"), h($, x, Be, "\u02DC", "\\~"), h($, x, Be, "\u02C9", "\\="), h($, x, Be, "\u02D8", "\\u"), h($, x, Be, "\u02D9", "\\."), h($, x, Be, "\xB8", "\\c"), h($, x, Be, "\u02DA", "\\r"), h($, x, Be, "\u02C7", "\\v"), h($, x, Be, "\xA8", '\\"'), h($, x, Be, "\u02DD", "\\H"), h($, x, Be, "\u25EF", "\\textcircled");
+            let Ii = {
                 "--": !0,
                 "---": !0,
                 "``": !0,
                 "''": !0
             };
-            h(H, x, D, "\u2013", "--", !0), h(H, x, D, "\u2013", "\\textendash"), h(H, x, D, "\u2014", "---", !0), h(H, x, D, "\u2014", "\\textemdash"), h(H, x, D, "\u2018", "`", !0), h(H, x, D, "\u2018", "\\textquoteleft"), h(H, x, D, "\u2019", "'", !0), h(H, x, D, "\u2019", "\\textquoteright"), h(H, x, D, "\u201C", "``", !0), h(H, x, D, "\u201C", "\\textquotedblleft"), h(H, x, D, "\u201D", "''", !0), h(H, x, D, "\u201D", "\\textquotedblright"), h(p, x, D, "\xB0", "\\degree", !0), h(H, x, D, "\xB0", "\\degree"), h(H, x, D, "\xB0", "\\textdegree", !0), h(p, x, D, "\xA3", "\\pounds"), h(p, x, D, "\xA3", "\\mathsterling", !0), h(H, x, D, "\xA3", "\\pounds"), h(H, x, D, "\xA3", "\\textsterling", !0), h(p, C, D, "\u2720", "\\maltese"), h(H, C, D, "\u2720", "\\maltese");
-            let Ni = '0123456789/@."';
-            for (let n = 0; n < Ni.length; n++) {
-                let t = Ni.charAt(n);
-                h(p, x, D, t, t)
-            }
-            let Li = '0123456789!@*()-=+";:?/.,';
-            for (let n = 0; n < Li.length; n++) {
-                let t = Li.charAt(n);
-                h(H, x, D, t, t)
-            }
-            let Vr = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz";
-            for (let n = 0; n < Vr.length; n++) {
-                let t = Vr.charAt(n);
-                h(p, x, se, t, t), h(H, x, D, t, t)
+            h($, x, D, "\u2013", "--", !0), h($, x, D, "\u2013", "\\textendash"), h($, x, D, "\u2014", "---", !0), h($, x, D, "\u2014", "\\textemdash"), h($, x, D, "\u2018", "`", !0), h($, x, D, "\u2018", "\\textquoteleft"), h($, x, D, "\u2019", "'", !0), h($, x, D, "\u2019", "\\textquoteright"), h($, x, D, "\u201C", "``", !0), h($, x, D, "\u201C", "\\textquotedblleft"), h($, x, D, "\u201D", "''", !0), h($, x, D, "\u201D", "\\textquotedblright"), h(m, x, D, "\xB0", "\\degree", !0), h($, x, D, "\xB0", "\\degree"), h($, x, D, "\xB0", "\\textdegree", !0), h(m, x, D, "\xA3", "\\pounds"), h(m, x, D, "\xA3", "\\mathsterling", !0), h($, x, D, "\xA3", "\\pounds"), h($, x, D, "\xA3", "\\textsterling", !0), h(m, C, D, "\u2720", "\\maltese"), h($, C, D, "\u2720", "\\maltese");
+            let Oi = '0123456789/@."';
+            for (let n = 0; n < Oi.length; n++) {
+                let t = Oi.charAt(n);
+                h(m, x, D, t, t)
+            }
+            let Hi = '0123456789!@*()-=+";:?/.,';
+            for (let n = 0; n < Hi.length; n++) {
+                let t = Hi.charAt(n);
+                h($, x, D, t, t)
+            }
+            let jr = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz";
+            for (let n = 0; n < jr.length; n++) {
+                let t = jr.charAt(n);
+                h(m, x, se, t, t), h($, x, D, t, t)
             }
-            h(p, C, D, "C", "\u2102"), h(H, C, D, "C", "\u2102"), h(p, C, D, "H", "\u210D"), h(H, C, D, "H", "\u210D"), h(p, C, D, "N", "\u2115"), h(H, C, D, "N", "\u2115"), h(p, C, D, "P", "\u2119"), h(H, C, D, "P", "\u2119"), h(p, C, D, "Q", "\u211A"), h(H, C, D, "Q", "\u211A"), h(p, C, D, "R", "\u211D"), h(H, C, D, "R", "\u211D"), h(p, C, D, "Z", "\u2124"), h(H, C, D, "Z", "\u2124"), h(p, x, se, "h", "\u210E"), h(H, x, se, "h", "\u210E");
+            h(m, C, D, "C", "\u2102"), h($, C, D, "C", "\u2102"), h(m, C, D, "H", "\u210D"), h($, C, D, "H", "\u210D"), h(m, C, D, "N", "\u2115"), h($, C, D, "N", "\u2115"), h(m, C, D, "P", "\u2119"), h($, C, D, "P", "\u2119"), h(m, C, D, "Q", "\u211A"), h($, C, D, "Q", "\u211A"), h(m, C, D, "R", "\u211D"), h($, C, D, "R", "\u211D"), h(m, C, D, "Z", "\u2124"), h($, C, D, "Z", "\u2124"), h(m, x, se, "h", "\u210E"), h($, x, se, "h", "\u210E");
             let le = "";
-            for (let n = 0; n < Vr.length; n++) {
-                let t = Vr.charAt(n);
-                le = String.fromCharCode(55349, 56320 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 56372 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 56424 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 56580 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 56684 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 56736 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 56788 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 56840 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 56944 + n), h(p, x, se, t, le), h(H, x, D, t, le), n < 26 && (le = String.fromCharCode(55349, 56632 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 56476 + n), h(p, x, se, t, le), h(H, x, D, t, le))
+            for (let n = 0; n < jr.length; n++) {
+                let t = jr.charAt(n);
+                le = String.fromCharCode(55349, 56320 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56372 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56424 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56580 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56684 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56736 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56788 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56840 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56944 + n), h(m, x, se, t, le), h($, x, D, t, le), n < 26 && (le = String.fromCharCode(55349, 56632 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 56476 + n), h(m, x, se, t, le), h($, x, D, t, le))
             }
-            le = "\u{1D55C}", h(p, x, se, "k", le), h(H, x, D, "k", le);
+            le = "\u{1D55C}", h(m, x, se, "k", le), h($, x, D, "k", le);
             for (let n = 0; n < 10; n++) {
                 let t = n.toString();
-                le = String.fromCharCode(55349, 57294 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 57314 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 57324 + n), h(p, x, se, t, le), h(H, x, D, t, le), le = String.fromCharCode(55349, 57334 + n), h(p, x, se, t, le), h(H, x, D, t, le)
+                le = String.fromCharCode(55349, 57294 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 57314 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 57324 + n), h(m, x, se, t, le), h($, x, D, t, le), le = String.fromCharCode(55349, 57334 + n), h(m, x, se, t, le), h($, x, D, t, le)
             }
-            let Y0 = "\xD0\xDE\xFE";
-            for (let n = 0; n < Y0.length; n++) {
-                let t = Y0.charAt(n);
-                h(p, x, se, t, t), h(H, x, D, t, t)
+            let Z0 = "\xD0\xDE\xFE";
+            for (let n = 0; n < Z0.length; n++) {
+                let t = Z0.charAt(n);
+                h(m, x, se, t, t), h($, x, D, t, t)
             }
-            let jr = [
+            let Ur = [
                     ["mathbf", "textbf", "Main-Bold"],
                     ["mathbf", "textbf", "Main-Bold"],
                     ["mathnormal", "textit", "Math-Italic"],
                     ["mathnormal", "textit", "Math-Italic"],
                     ["boldsymbol", "boldsymbol", "Main-BoldItalic"],
                     ["boldsymbol", "boldsymbol", "Main-BoldItalic"],
                     ["mathscr", "textscr", "Script-Regular"],
@@ -9070,169 +9070,169 @@
                     ["mathitsf", "textitsf", "SansSerif-Italic"],
                     ["mathitsf", "textitsf", "SansSerif-Italic"],
                     ["", "", ""],
                     ["", "", ""],
                     ["mathtt", "texttt", "Typewriter-Regular"],
                     ["mathtt", "texttt", "Typewriter-Regular"]
                 ],
-                Pi = [
+                $i = [
                     ["mathbf", "textbf", "Main-Bold"],
                     ["", "", ""],
                     ["mathsf", "textsf", "SansSerif-Regular"],
                     ["mathboldsf", "textboldsf", "SansSerif-Bold"],
                     ["mathtt", "texttt", "Typewriter-Regular"]
                 ],
-                Uu = function(n, t) {
+                Wu = function(n, t) {
                     let o = n.charCodeAt(0),
                         s = n.charCodeAt(1),
                         u = (o - 55296) * 1024 + (s - 56320) + 65536,
-                        f = t === "math" ? 0 : 1;
+                        p = t === "math" ? 0 : 1;
                     if (119808 <= u && u < 120484) {
                         let b = Math.floor((u - 119808) / 26);
-                        return [jr[b][2], jr[b][f]]
+                        return [Ur[b][2], Ur[b][p]]
                     } else if (120782 <= u && u <= 120831) {
                         let b = Math.floor((u - 120782) / 10);
-                        return [Pi[b][2], Pi[b][f]]
+                        return [$i[b][2], $i[b][p]]
                     } else {
-                        if (u === 120485 || u === 120486) return [jr[0][2], jr[0][f]];
+                        if (u === 120485 || u === 120486) return [Ur[0][2], Ur[0][p]];
                         if (120486 < u && u < 120782) return ["", ""];
                         throw new a("Unsupported character: " + n)
                     }
                 },
-                Ur = function(n, t, o) {
+                Wr = function(n, t, o) {
                     return Oe[o][n] && Oe[o][n].replace && (n = Oe[o][n].replace), {
                         value: n,
-                        metrics: G0(n, t, o)
+                        metrics: V0(n, t, o)
                     }
                 },
                 yt = function(n, t, o, s, u) {
-                    let f = Ur(n, t, o),
-                        b = f.metrics;
-                    n = f.value;
+                    let p = Wr(n, t, o),
+                        b = p.metrics;
+                    n = p.value;
                     let v;
                     if (b) {
                         let S = b.italic;
                         (o === "text" || s && s.font === "mathit") && (S = 0), v = new ut(n, b.height, b.depth, S, b.skew, b.width, u)
                     } else typeof console < "u" && console.warn("No character metrics " + ("for '" + n + "' in style '" + t + "' and mode '" + o + "'")), v = new ut(n, 0, 0, 0, 0, 0, u);
                     if (s) {
                         v.maxFontSize = s.sizeMultiplier, s.style.isTight() && v.classes.push("mtight");
                         let S = s.getColor();
                         S && (v.style.color = S)
                     }
                     return v
                 },
-                Wu = function(n, t, o, s) {
-                    return s === void 0 && (s = []), o.font === "boldsymbol" && Ur(n, "Main-Bold", t).metrics ? yt(n, "Main-Bold", t, o, s.concat(["mathbf"])) : n === "\\" || Oe[t][n].font === "main" ? yt(n, "Main-Regular", t, o, s) : yt(n, "AMS-Regular", t, o, s.concat(["amsrm"]))
+                Yu = function(n, t, o, s) {
+                    return s === void 0 && (s = []), o.font === "boldsymbol" && Wr(n, "Main-Bold", t).metrics ? yt(n, "Main-Bold", t, o, s.concat(["mathbf"])) : n === "\\" || Oe[t][n].font === "main" ? yt(n, "Main-Regular", t, o, s) : yt(n, "AMS-Regular", t, o, s.concat(["amsrm"]))
                 },
-                Yu = function(n, t, o, s, u) {
-                    return u !== "textord" && Ur(n, "Math-BoldItalic", t).metrics ? {
+                Zu = function(n, t, o, s, u) {
+                    return u !== "textord" && Wr(n, "Math-BoldItalic", t).metrics ? {
                         fontName: "Math-BoldItalic",
                         fontClass: "boldsymbol"
                     } : {
                         fontName: "Main-Bold",
                         fontClass: "mathbf"
                     }
                 },
                 Qu = function(n, t, o) {
                     let s = n.mode,
                         u = n.text,
-                        f = ["mord"],
+                        p = ["mord"],
                         b = s === "math" || s === "text" && t.font,
                         v = b ? t.font : t.fontFamily,
                         S = "",
                         E = "";
-                    if (u.charCodeAt(0) === 55349 && ([S, E] = Uu(u, s)), S.length > 0) return yt(u, S, s, t, f.concat(E));
+                    if (u.charCodeAt(0) === 55349 && ([S, E] = Wu(u, s)), S.length > 0) return yt(u, S, s, t, p.concat(E));
                     if (v) {
                         let z, F;
                         if (v === "boldsymbol") {
-                            let N = Yu(u, s, t, f, o);
+                            let N = Zu(u, s, t, p, o);
                             z = N.fontName, F = [N.fontClass]
-                        } else b ? (z = Hi[v].fontName, F = [v]) : (z = Wr(v, t.fontWeight, t.fontShape), F = [v, t.fontWeight, t.fontShape]);
-                        if (Ur(u, z, s).metrics) return yt(u, z, s, t, f.concat(F));
-                        if (Bi.hasOwnProperty(u) && z.slice(0, 10) === "Typewriter") {
+                        } else b ? (z = ji[v].fontName, F = [v]) : (z = Yr(v, t.fontWeight, t.fontShape), F = [v, t.fontWeight, t.fontShape]);
+                        if (Wr(u, z, s).metrics) return yt(u, z, s, t, p.concat(F));
+                        if (Ii.hasOwnProperty(u) && z.slice(0, 10) === "Typewriter") {
                             let N = [];
-                            for (let O = 0; O < u.length; O++) N.push(yt(u[O], z, s, t, f.concat(F)));
-                            return Oi(N)
+                            for (let H = 0; H < u.length; H++) N.push(yt(u[H], z, s, t, p.concat(F)));
+                            return Vi(N)
                         }
                     }
-                    if (o === "mathord") return yt(u, "Math-Italic", s, t, f.concat(["mathnormal"]));
+                    if (o === "mathord") return yt(u, "Math-Italic", s, t, p.concat(["mathnormal"]));
                     if (o === "textord") {
                         let z = Oe[s][u] && Oe[s][u].font;
                         if (z === "ams") {
-                            let F = Wr("amsrm", t.fontWeight, t.fontShape);
-                            return yt(u, F, s, t, f.concat("amsrm", t.fontWeight, t.fontShape))
+                            let F = Yr("amsrm", t.fontWeight, t.fontShape);
+                            return yt(u, F, s, t, p.concat("amsrm", t.fontWeight, t.fontShape))
                         } else if (z === "main" || !z) {
-                            let F = Wr("textrm", t.fontWeight, t.fontShape);
-                            return yt(u, F, s, t, f.concat(t.fontWeight, t.fontShape))
+                            let F = Yr("textrm", t.fontWeight, t.fontShape);
+                            return yt(u, F, s, t, p.concat(t.fontWeight, t.fontShape))
                         } else {
-                            let F = Wr(z, t.fontWeight, t.fontShape);
-                            return yt(u, F, s, t, f.concat(F, t.fontWeight, t.fontShape))
+                            let F = Yr(z, t.fontWeight, t.fontShape);
+                            return yt(u, F, s, t, p.concat(F, t.fontWeight, t.fontShape))
                         }
                     } else throw new Error("unexpected type: " + o + " in makeOrd")
                 },
-                Zu = (n, t) => {
+                Xu = (n, t) => {
                     if (It(n.classes) !== It(t.classes) || n.skew !== t.skew || n.maxFontSize !== t.maxFontSize) return !1;
                     if (n.classes.length === 1) {
                         let o = n.classes[0];
                         if (o === "mbin" || o === "mord") return !1
                     }
                     for (let o in n.style)
                         if (n.style.hasOwnProperty(o) && n.style[o] !== t.style[o]) return !1;
                     for (let o in t.style)
                         if (t.style.hasOwnProperty(o) && n.style[o] !== t.style[o]) return !1;
                     return !0
                 },
-                Xu = n => {
+                Ju = n => {
                     for (let t = 0; t < n.length - 1; t++) {
                         let o = n[t],
                             s = n[t + 1];
-                        o instanceof ut && s instanceof ut && Zu(o, s) && (o.text += s.text, o.height = Math.max(o.height, s.height), o.depth = Math.max(o.depth, s.depth), o.italic = s.italic, n.splice(t + 1, 1), t--)
+                        o instanceof ut && s instanceof ut && Xu(o, s) && (o.text += s.text, o.height = Math.max(o.height, s.height), o.depth = Math.max(o.depth, s.depth), o.italic = s.italic, n.splice(t + 1, 1), t--)
                     }
                     return n
                 },
                 Q0 = function(n) {
                     let t = 0,
                         o = 0,
                         s = 0;
                     for (let u = 0; u < n.children.length; u++) {
-                        let f = n.children[u];
-                        f.height > t && (t = f.height), f.depth > o && (o = f.depth), f.maxFontSize > s && (s = f.maxFontSize)
+                        let p = n.children[u];
+                        p.height > t && (t = p.height), p.depth > o && (o = p.depth), p.maxFontSize > s && (s = p.maxFontSize)
                     }
                     n.height = t, n.depth = o, n.maxFontSize = s
                 },
                 nt = function(n, t, o, s) {
                     let u = new vr(n, t, o, s);
                     return Q0(u), u
                 },
-                Ii = (n, t, o, s) => new vr(n, t, o, s),
-                Ju = function(n, t, o) {
+                Gi = (n, t, o, s) => new vr(n, t, o, s),
+                Ku = function(n, t, o) {
                     let s = nt([n], [], t);
-                    return s.height = Math.max(o || t.fontMetrics().defaultRuleThickness, t.minRuleThickness), s.style.borderBottomWidth = Q(s.height), s.maxFontSize = 1, s
+                    return s.height = Math.max(o || t.fontMetrics().defaultRuleThickness, t.minRuleThickness), s.style.borderBottomWidth = Z(s.height), s.maxFontSize = 1, s
                 },
-                Ku = function(n, t, o, s) {
-                    let u = new U0(n, t, o, s);
+                e1 = function(n, t, o, s) {
+                    let u = new W0(n, t, o, s);
                     return Q0(u), u
                 },
-                Oi = function(n) {
+                Vi = function(n) {
                     let t = new xr(n);
                     return Q0(t), t
                 },
-                e1 = function(n, t) {
+                t1 = function(n, t) {
                     return n instanceof xr ? nt([], [n], t) : n
                 },
-                t1 = function(n) {
+                r1 = function(n) {
                     if (n.positionType === "individualShift") {
                         let o = n.children,
                             s = [o[0]],
                             u = -o[0].shift - o[0].elem.depth,
-                            f = u;
+                            p = u;
                         for (let b = 1; b < o.length; b++) {
-                            let v = -o[b].shift - f - o[b].elem.depth,
+                            let v = -o[b].shift - p - o[b].elem.depth,
                                 S = v - (o[b - 1].elem.height + o[b - 1].elem.depth);
-                            f = f + v, s.push({
+                            p = p + v, s.push({
                                 type: "kern",
                                 size: S
                             }), s.push(o[b])
                         }
                         return {
                             children: s,
                             depth: u
@@ -9255,64 +9255,64 @@
                         else throw new Error("Invalid positionType " + n.positionType + ".")
                     }
                     return {
                         children: n.children,
                         depth: t
                     }
                 },
-                r1 = function(n, t) {
+                n1 = function(n, t) {
                     let {
                         children: o,
                         depth: s
-                    } = t1(n), u = 0;
-                    for (let O = 0; O < o.length; O++) {
-                        let K = o[O];
+                    } = r1(n), u = 0;
+                    for (let H = 0; H < o.length; H++) {
+                        let K = o[H];
                         if (K.type === "elem") {
                             let ie = K.elem;
                             u = Math.max(u, ie.maxFontSize, ie.height)
                         }
                     }
                     u += 2;
-                    let f = nt(["pstrut"], []);
-                    f.style.height = Q(u);
+                    let p = nt(["pstrut"], []);
+                    p.style.height = Z(u);
                     let b = [],
                         v = s,
                         S = s,
                         E = s;
-                    for (let O = 0; O < o.length; O++) {
-                        let K = o[O];
+                    for (let H = 0; H < o.length; H++) {
+                        let K = o[H];
                         if (K.type === "kern") E += K.size;
                         else {
                             let ie = K.elem,
                                 ye = K.wrapperClasses || [],
                                 ge = K.wrapperStyle || {},
-                                xe = nt(ye, [f, ie], void 0, ge);
-                            xe.style.top = Q(-u - E - ie.depth), K.marginLeft && (xe.style.marginLeft = K.marginLeft), K.marginRight && (xe.style.marginRight = K.marginRight), b.push(xe), E += ie.height + ie.depth
+                                xe = nt(ye, [p, ie], void 0, ge);
+                            xe.style.top = Z(-u - E - ie.depth), K.marginLeft && (xe.style.marginLeft = K.marginLeft), K.marginRight && (xe.style.marginRight = K.marginRight), b.push(xe), E += ie.height + ie.depth
                         }
                         v = Math.min(v, E), S = Math.max(S, E)
                     }
                     let z = nt(["vlist"], b);
-                    z.style.height = Q(S);
+                    z.style.height = Z(S);
                     let F;
                     if (v < 0) {
-                        let O = nt([], []),
-                            K = nt(["vlist"], [O]);
-                        K.style.height = Q(-v);
+                        let H = nt([], []),
+                            K = nt(["vlist"], [H]);
+                        K.style.height = Z(-v);
                         let ie = nt(["vlist-s"], [new ut("\u200B")]);
                         F = [nt(["vlist-r"], [z, ie]), nt(["vlist-r"], [K])]
                     } else F = [nt(["vlist-r"], [z])];
                     let N = nt(["vlist-t"], F);
                     return F.length === 2 && N.classes.push("vlist-t2"), N.height = S, N.depth = -v, N
                 },
-                n1 = (n, t) => {
+                i1 = (n, t) => {
                     let o = nt(["mspace"], [], t),
                         s = Ie(n, t);
-                    return o.style.marginRight = Q(s), o
+                    return o.style.marginRight = Z(s), o
                 },
-                Wr = function(n, t, o) {
+                Yr = function(n, t, o) {
                     let s = "";
                     switch (n) {
                         case "amsrm":
                             s = "AMS";
                             break;
                         case "textrm":
                             s = "Main";
@@ -9325,15 +9325,15 @@
                             break;
                         default:
                             s = n
                     }
                     let u;
                     return t === "textbf" && o === "textit" ? u = "BoldItalic" : t === "textbf" ? u = "Bold" : t === "textit" ? u = "Italic" : u = "Regular", s + "-" + u
                 },
-                Hi = {
+                ji = {
                     mathbf: {
                         variant: "bold",
                         fontName: "Main-Bold"
                     },
                     mathrm: {
                         variant: "normal",
                         fontName: "Main-Regular"
@@ -9371,88 +9371,88 @@
                         fontName: "SansSerif-Regular"
                     },
                     mathtt: {
                         variant: "monospace",
                         fontName: "Typewriter-Regular"
                     }
                 },
-                $i = {
+                Ui = {
                     vec: ["vec", .471, .714],
                     oiintSize1: ["oiintSize1", .957, .499],
                     oiintSize2: ["oiintSize2", 1.472, .659],
                     oiiintSize1: ["oiiintSize1", 1.304, .499],
                     oiiintSize2: ["oiiintSize2", 1.98, .659]
                 };
             var B = {
-                fontMap: Hi,
+                fontMap: ji,
                 makeSymbol: yt,
-                mathsym: Wu,
+                mathsym: Yu,
                 makeSpan: nt,
-                makeSvgSpan: Ii,
-                makeLineSpan: Ju,
-                makeAnchor: Ku,
-                makeFragment: Oi,
-                wrapFragment: e1,
-                makeVList: r1,
+                makeSvgSpan: Gi,
+                makeLineSpan: Ku,
+                makeAnchor: e1,
+                makeFragment: Vi,
+                wrapFragment: t1,
+                makeVList: n1,
                 makeOrd: Qu,
-                makeGlue: n1,
+                makeGlue: i1,
                 staticSvg: function(n, t) {
-                    let [o, s, u] = $i[n], f = new Ot(o), b = new Et([f], {
-                        width: Q(s),
-                        height: Q(u),
-                        style: "width:" + Q(s),
+                    let [o, s, u] = Ui[n], p = new Ot(o), b = new Et([p], {
+                        width: Z(s),
+                        height: Z(u),
+                        style: "width:" + Z(s),
                         viewBox: "0 0 " + 1e3 * s + " " + 1e3 * u,
                         preserveAspectRatio: "xMinYMin"
-                    }), v = Ii(["overlay"], [b], t);
-                    return v.height = u, v.style.height = Q(u), v.style.width = Q(s), v
+                    }), v = Gi(["overlay"], [b], t);
+                    return v.height = u, v.style.height = Z(u), v.style.width = Z(s), v
                 },
-                svgData: $i,
-                tryCombineChars: Xu
+                svgData: Ui,
+                tryCombineChars: Ju
             };
             let He = {
                     number: 3,
                     unit: "mu"
                 },
-                Xt = {
+                Jt = {
                     number: 4,
                     unit: "mu"
                 },
                 zt = {
                     number: 5,
                     unit: "mu"
                 },
-                i1 = {
+                o1 = {
                     mord: {
                         mop: He,
-                        mbin: Xt,
+                        mbin: Jt,
                         mrel: zt,
                         minner: He
                     },
                     mop: {
                         mord: He,
                         mop: He,
                         mrel: zt,
                         minner: He
                     },
                     mbin: {
-                        mord: Xt,
-                        mop: Xt,
-                        mopen: Xt,
-                        minner: Xt
+                        mord: Jt,
+                        mop: Jt,
+                        mopen: Jt,
+                        minner: Jt
                     },
                     mrel: {
                         mord: zt,
                         mop: zt,
                         mopen: zt,
                         minner: zt
                     },
                     mopen: {},
                     mclose: {
                         mop: He,
-                        mbin: Xt,
+                        mbin: Jt,
                         mrel: zt,
                         minner: He
                     },
                     mpunct: {
                         mord: He,
                         mop: He,
                         mrel: zt,
@@ -9460,22 +9460,22 @@
                         mclose: He,
                         mpunct: He,
                         minner: He
                     },
                     minner: {
                         mord: He,
                         mop: He,
-                        mbin: Xt,
+                        mbin: Jt,
                         mrel: zt,
                         mopen: He,
                         mpunct: He,
                         minner: He
                     }
                 },
-                o1 = {
+                a1 = {
                     mord: {
                         mop: He
                     },
                     mop: {
                         mord: He,
                         mop: He
                     },
@@ -9486,207 +9486,207 @@
                         mop: He
                     },
                     mpunct: {},
                     minner: {
                         mop: He
                     }
                 },
-                Gi = {},
-                Yr = {},
+                Wi = {},
+                Zr = {},
                 Qr = {};
 
-            function Z(n) {
+            function Q(n) {
                 let {
                     type: t,
                     names: o,
                     props: s,
                     handler: u,
-                    htmlBuilder: f,
+                    htmlBuilder: p,
                     mathmlBuilder: b
                 } = n, v = {
                     type: t,
                     numArgs: s.numArgs,
                     argTypes: s.argTypes,
                     allowedInArgument: !!s.allowedInArgument,
                     allowedInText: !!s.allowedInText,
                     allowedInMath: s.allowedInMath === void 0 ? !0 : s.allowedInMath,
                     numOptionalArgs: s.numOptionalArgs || 0,
                     infix: !!s.infix,
                     primitive: !!s.primitive,
                     handler: u
                 };
-                for (let S = 0; S < o.length; ++S) Gi[o[S]] = v;
-                t && (f && (Yr[t] = f), b && (Qr[t] = b))
+                for (let S = 0; S < o.length; ++S) Wi[o[S]] = v;
+                t && (p && (Zr[t] = p), b && (Qr[t] = b))
             }
 
-            function Jt(n) {
+            function Kt(n) {
                 let {
                     type: t,
                     htmlBuilder: o,
                     mathmlBuilder: s
                 } = n;
-                Z({
+                Q({
                     type: t,
                     names: [],
                     props: {
                         numArgs: 0
                     },
                     handler() {
                         throw new Error("Should never be called.")
                     },
                     htmlBuilder: o,
                     mathmlBuilder: s
                 })
             }
-            let Zr = function(n) {
+            let Xr = function(n) {
                     return n.type === "ordgroup" && n.body.length === 1 ? n.body[0] : n
                 },
                 je = function(n) {
                     return n.type === "ordgroup" ? n.body : [n]
                 },
                 Rt = B.makeSpan,
-                a1 = ["leftmost", "mbin", "mopen", "mrel", "mop", "mpunct"],
-                s1 = ["rightmost", "mrel", "mclose", "mpunct"],
-                l1 = {
-                    display: $.DISPLAY,
-                    text: $.TEXT,
-                    script: $.SCRIPT,
-                    scriptscript: $.SCRIPTSCRIPT
-                },
+                s1 = ["leftmost", "mbin", "mopen", "mrel", "mop", "mpunct"],
+                l1 = ["rightmost", "mrel", "mclose", "mpunct"],
                 c1 = {
+                    display: G.DISPLAY,
+                    text: G.TEXT,
+                    script: G.SCRIPT,
+                    scriptscript: G.SCRIPTSCRIPT
+                },
+                u1 = {
                     mord: "mord",
                     mop: "mop",
                     mbin: "mbin",
                     mrel: "mrel",
                     mopen: "mopen",
                     mclose: "mclose",
                     mpunct: "mpunct",
                     minner: "minner"
                 },
-                Qe = function(n, t, o, s) {
+                Ze = function(n, t, o, s) {
                     s === void 0 && (s = [null, null]);
                     let u = [];
                     for (let E = 0; E < n.length; E++) {
                         let z = ve(n[E], t);
                         if (z instanceof xr) {
                             let F = z.children;
                             u.push(...F)
                         } else u.push(z)
                     }
                     if (B.tryCombineChars(u), !o) return u;
-                    let f = t;
+                    let p = t;
                     if (n.length === 1) {
                         let E = n[0];
-                        E.type === "sizing" ? f = t.havingSize(E.size) : E.type === "styling" && (f = t.havingStyle(l1[E.style]))
+                        E.type === "sizing" ? p = t.havingSize(E.size) : E.type === "styling" && (p = t.havingStyle(c1[E.style]))
                     }
                     let b = Rt([s[0] || "leftmost"], [], t),
                         v = Rt([s[1] || "rightmost"], [], t),
                         S = o === "root";
-                    return Z0(u, (E, z) => {
+                    return X0(u, (E, z) => {
                         let F = z.classes[0],
                             N = E.classes[0];
-                        F === "mbin" && R.contains(s1, N) ? z.classes[0] = "mord" : N === "mbin" && R.contains(a1, F) && (E.classes[0] = "mord")
+                        F === "mbin" && R.contains(l1, N) ? z.classes[0] = "mord" : N === "mbin" && R.contains(s1, F) && (E.classes[0] = "mord")
                     }, {
                         node: b
-                    }, v, S), Z0(u, (E, z) => {
-                        let F = J0(z),
-                            N = J0(E),
-                            O = F && N ? E.hasClass("mtight") ? o1[F][N] : i1[F][N] : null;
-                        if (O) return B.makeGlue(O, f)
+                    }, v, S), X0(u, (E, z) => {
+                        let F = K0(z),
+                            N = K0(E),
+                            H = F && N ? E.hasClass("mtight") ? a1[F][N] : o1[F][N] : null;
+                        if (H) return B.makeGlue(H, p)
                     }, {
                         node: b
                     }, v, S), u
                 },
-                Z0 = function(n, t, o, s, u) {
+                X0 = function(n, t, o, s, u) {
                     s && n.push(s);
-                    let f = 0;
-                    for (; f < n.length; f++) {
-                        let b = n[f],
-                            v = Vi(b);
+                    let p = 0;
+                    for (; p < n.length; p++) {
+                        let b = n[p],
+                            v = Yi(b);
                         if (v) {
-                            Z0(v.children, t, o, null, u);
+                            X0(v.children, t, o, null, u);
                             continue
                         }
                         let S = !b.hasClass("mspace");
                         if (S) {
                             let E = t(b, o.node);
-                            E && (o.insertAfter ? o.insertAfter(E) : (n.unshift(E), f++))
+                            E && (o.insertAfter ? o.insertAfter(E) : (n.unshift(E), p++))
                         }
                         S ? o.node = b : u && b.hasClass("newline") && (o.node = Rt(["leftmost"])), o.insertAfter = (E => z => {
-                            n.splice(E + 1, 0, z), f++
-                        })(f)
+                            n.splice(E + 1, 0, z), p++
+                        })(p)
                     }
                     s && n.pop()
                 },
-                Vi = function(n) {
-                    return n instanceof xr || n instanceof U0 || n instanceof vr && n.hasClass("enclosing") ? n : null
+                Yi = function(n) {
+                    return n instanceof xr || n instanceof W0 || n instanceof vr && n.hasClass("enclosing") ? n : null
                 },
-                X0 = function(n, t) {
-                    let o = Vi(n);
+                J0 = function(n, t) {
+                    let o = Yi(n);
                     if (o) {
                         let s = o.children;
                         if (s.length) {
-                            if (t === "right") return X0(s[s.length - 1], "right");
-                            if (t === "left") return X0(s[0], "left")
+                            if (t === "right") return J0(s[s.length - 1], "right");
+                            if (t === "left") return J0(s[0], "left")
                         }
                     }
                     return n
                 },
-                J0 = function(n, t) {
-                    return n ? (t && (n = X0(n, t)), c1[n.classes[0]] || null) : null
+                K0 = function(n, t) {
+                    return n ? (t && (n = J0(n, t)), u1[n.classes[0]] || null) : null
                 },
                 wr = function(n, t) {
                     let o = ["nulldelimiter"].concat(n.baseSizingClasses());
                     return Rt(t.concat(o))
                 },
                 ve = function(n, t, o) {
                     if (!n) return Rt();
-                    if (Yr[n.type]) {
-                        let s = Yr[n.type](n, t);
+                    if (Zr[n.type]) {
+                        let s = Zr[n.type](n, t);
                         if (o && t.size !== o.size) {
                             s = Rt(t.sizingClasses(o), [s], t);
                             let u = t.sizeMultiplier / o.sizeMultiplier;
                             s.height *= u, s.depth *= u
                         }
                         return s
                     } else throw new a("Got group of unknown type: '" + n.type + "'")
                 };
 
-            function Xr(n, t) {
+            function Jr(n, t) {
                 let o = Rt(["base"], n, t),
                     s = Rt(["strut"]);
-                return s.style.height = Q(o.height + o.depth), o.depth && (s.style.verticalAlign = Q(-o.depth)), o.children.unshift(s), o
+                return s.style.height = Z(o.height + o.depth), o.depth && (s.style.verticalAlign = Z(-o.depth)), o.children.unshift(s), o
             }
 
-            function K0(n, t) {
+            function en(n, t) {
                 let o = null;
                 n.length === 1 && n[0].type === "tag" && (o = n[0].tag, n = n[0].body);
-                let s = Qe(n, t, "root"),
+                let s = Ze(n, t, "root"),
                     u;
                 s.length === 2 && s[1].hasClass("tag") && (u = s.pop());
-                let f = [],
+                let p = [],
                     b = [];
                 for (let E = 0; E < s.length; E++)
                     if (b.push(s[E]), s[E].hasClass("mbin") || s[E].hasClass("mrel") || s[E].hasClass("allowbreak")) {
                         let z = !1;
                         for (; E < s.length - 1 && s[E + 1].hasClass("mspace") && !s[E + 1].hasClass("newline");) E++, b.push(s[E]), s[E].hasClass("nobreak") && (z = !0);
-                        z || (f.push(Xr(b, t)), b = [])
-                    } else s[E].hasClass("newline") && (b.pop(), b.length > 0 && (f.push(Xr(b, t)), b = []), f.push(s[E]));
-                b.length > 0 && f.push(Xr(b, t));
+                        z || (p.push(Jr(b, t)), b = [])
+                    } else s[E].hasClass("newline") && (b.pop(), b.length > 0 && (p.push(Jr(b, t)), b = []), p.push(s[E]));
+                b.length > 0 && p.push(Jr(b, t));
                 let v;
-                o ? (v = Xr(Qe(o, t, !0)), v.classes = ["tag"], f.push(v)) : u && f.push(u);
-                let S = Rt(["katex-html"], f);
+                o ? (v = Jr(Ze(o, t, !0)), v.classes = ["tag"], p.push(v)) : u && p.push(u);
+                let S = Rt(["katex-html"], p);
                 if (S.setAttribute("aria-hidden", "true"), v) {
                     let E = v.children[0];
-                    E.style.height = Q(S.height + S.depth), S.depth && (E.style.verticalAlign = Q(-S.depth))
+                    E.style.height = Z(S.height + S.depth), S.depth && (E.style.verticalAlign = Z(-S.depth))
                 }
                 return S
             }
 
-            function ji(n) {
+            function Zi(n) {
                 return new xr(n)
             }
             class ht {
                 constructor(t, o, s) {
                     this.type = void 0, this.attributes = void 0, this.children = void 0, this.classes = void 0, this.type = t, this.attributes = {}, this.children = o || [], this.classes = s || []
                 }
                 setAttribute(t, o) {
@@ -9723,45 +9723,45 @@
                 toMarkup() {
                     return R.escape(this.toText())
                 }
                 toText() {
                     return this.text
                 }
             }
-            class u1 {
+            class h1 {
                 constructor(t) {
                     this.width = void 0, this.character = void 0, this.width = t, t >= .05555 && t <= .05556 ? this.character = "\u200A" : t >= .1666 && t <= .1667 ? this.character = "\u2009" : t >= .2222 && t <= .2223 ? this.character = "\u2005" : t >= .2777 && t <= .2778 ? this.character = "\u2005\u200A" : t >= -.05556 && t <= -.05555 ? this.character = "\u200A\u2063" : t >= -.1667 && t <= -.1666 ? this.character = "\u2009\u2063" : t >= -.2223 && t <= -.2222 ? this.character = "\u205F\u2063" : t >= -.2778 && t <= -.2777 ? this.character = "\u2005\u2063" : this.character = null
                 }
                 toNode() {
                     if (this.character) return document.createTextNode(this.character);
                     {
                         let t = document.createElementNS("http://www.w3.org/1998/Math/MathML", "mspace");
-                        return t.setAttribute("width", Q(this.width)), t
+                        return t.setAttribute("width", Z(this.width)), t
                     }
                 }
                 toMarkup() {
-                    return this.character ? "<mtext>" + this.character + "</mtext>" : '<mspace width="' + Q(this.width) + '"/>'
+                    return this.character ? "<mtext>" + this.character + "</mtext>" : '<mspace width="' + Z(this.width) + '"/>'
                 }
                 toText() {
                     return this.character ? this.character : " "
                 }
             }
             var V = {
                 MathNode: ht,
                 TextNode: kr,
-                SpaceNode: u1,
-                newDocumentFragment: ji
+                SpaceNode: h1,
+                newDocumentFragment: Zi
             };
             let dt = function(n, t, o) {
-                    return Oe[t][n] && Oe[t][n].replace && n.charCodeAt(0) !== 55349 && !(Bi.hasOwnProperty(n) && o && (o.fontFamily && o.fontFamily.slice(4, 6) === "tt" || o.font && o.font.slice(4, 6) === "tt")) && (n = Oe[t][n].replace), new V.TextNode(n)
+                    return Oe[t][n] && Oe[t][n].replace && n.charCodeAt(0) !== 55349 && !(Ii.hasOwnProperty(n) && o && (o.fontFamily && o.fontFamily.slice(4, 6) === "tt" || o.font && o.font.slice(4, 6) === "tt")) && (n = Oe[t][n].replace), new V.TextNode(n)
                 },
-                en = function(n) {
+                tn = function(n) {
                     return n.length === 1 ? n[0] : new V.MathNode("mrow", n)
                 },
-                tn = function(n, t) {
+                rn = function(n, t) {
                     if (t.fontFamily === "texttt") return "monospace";
                     if (t.fontFamily === "textsf") return t.fontShape === "textit" && t.fontWeight === "textbf" ? "sans-serif-bold-italic" : t.fontShape === "textit" ? "sans-serif-italic" : t.fontWeight === "textbf" ? "bold-sans-serif" : "sans-serif";
                     if (t.fontShape === "textit" && t.fontWeight === "textbf") return "bold-italic";
                     if (t.fontShape === "textit") return "italic";
                     if (t.fontWeight === "textbf") return "bold";
                     let o = t.font;
                     if (!o || o === "mathnormal") return null;
@@ -9773,26 +9773,26 @@
                     if (o === "mathfrak") return "fraktur";
                     if (o === "mathscr" || o === "mathcal") return "script";
                     if (o === "mathsf") return "sans-serif";
                     if (o === "mathtt") return "monospace";
                     let u = n.text;
                     if (R.contains(["\\imath", "\\jmath"], u)) return null;
                     Oe[s][u] && Oe[s][u].replace && (u = Oe[s][u].replace);
-                    let f = B.fontMap[o].fontName;
-                    return G0(u, f, s) ? B.fontMap[o].variant : null
+                    let p = B.fontMap[o].fontName;
+                    return V0(u, p, s) ? B.fontMap[o].variant : null
                 },
                 it = function(n, t, o) {
                     if (n.length === 1) {
-                        let f = Ee(n[0], t);
-                        return o && f instanceof ht && f.type === "mo" && (f.setAttribute("lspace", "0em"), f.setAttribute("rspace", "0em")), [f]
+                        let p = Ee(n[0], t);
+                        return o && p instanceof ht && p.type === "mo" && (p.setAttribute("lspace", "0em"), p.setAttribute("rspace", "0em")), [p]
                     }
                     let s = [],
                         u;
-                    for (let f = 0; f < n.length; f++) {
-                        let b = Ee(n[f], t);
+                    for (let p = 0; p < n.length; p++) {
+                        let b = Ee(n[p], t);
                         if (b instanceof ht && u instanceof ht) {
                             if (b.type === "mtext" && u.type === "mtext" && b.getAttribute("mathvariant") === u.getAttribute("mathvariant")) {
                                 u.children.push(...b.children);
                                 continue
                             } else if (b.type === "mn" && u.type === "mn") {
                                 u.children.push(...b.children);
                                 continue
@@ -9811,70 +9811,70 @@
                             }
                         }
                         s.push(b), u = b
                     }
                     return s
                 },
                 Ht = function(n, t, o) {
-                    return en(it(n, t, o))
+                    return tn(it(n, t, o))
                 },
                 Ee = function(n, t) {
                     if (!n) return new V.MathNode("mrow");
                     if (Qr[n.type]) return Qr[n.type](n, t);
                     throw new a("Got group of unknown type: '" + n.type + "'")
                 };
 
-            function Ui(n, t, o, s, u) {
-                let f = it(n, o),
+            function Qi(n, t, o, s, u) {
+                let p = it(n, o),
                     b;
-                f.length === 1 && f[0] instanceof ht && R.contains(["mrow", "mtable"], f[0].type) ? b = f[0] : b = new V.MathNode("mrow", f);
+                p.length === 1 && p[0] instanceof ht && R.contains(["mrow", "mtable"], p[0].type) ? b = p[0] : b = new V.MathNode("mrow", p);
                 let v = new V.MathNode("annotation", [new V.TextNode(t)]);
                 v.setAttribute("encoding", "application/x-tex");
                 let S = new V.MathNode("semantics", [b, v]),
                     E = new V.MathNode("math", [S]);
                 E.setAttribute("xmlns", "http://www.w3.org/1998/Math/MathML"), s && E.setAttribute("display", "block");
                 let z = u ? "katex" : "katex-mathml";
                 return B.makeSpan([z], [E])
             }
-            let Wi = function(n) {
-                    return new Iu({
-                        style: n.displayMode ? $.DISPLAY : $.TEXT,
+            let Xi = function(n) {
+                    return new Ou({
+                        style: n.displayMode ? G.DISPLAY : G.TEXT,
                         maxSize: n.maxSize,
                         minRuleThickness: n.minRuleThickness
                     })
                 },
-                Yi = function(n, t) {
+                Ji = function(n, t) {
                     if (t.displayMode) {
                         let o = ["katex-display"];
                         t.leqno && o.push("leqno"), t.fleqn && o.push("fleqn"), n = B.makeSpan(o, [n])
                     }
                     return n
                 },
-                h1 = function(n, t, o) {
-                    let s = Wi(o),
+                d1 = function(n, t, o) {
+                    let s = Xi(o),
                         u;
-                    if (o.output === "mathml") return Ui(n, t, s, o.displayMode, !0);
+                    if (o.output === "mathml") return Qi(n, t, s, o.displayMode, !0);
                     if (o.output === "html") {
-                        let f = K0(n, s);
-                        u = B.makeSpan(["katex"], [f])
+                        let p = en(n, s);
+                        u = B.makeSpan(["katex"], [p])
                     } else {
-                        let f = Ui(n, t, s, o.displayMode, !1),
-                            b = K0(n, s);
-                        u = B.makeSpan(["katex"], [f, b])
-                    }
-                    return Yi(u, o)
-                },
-                d1 = function(n, t, o) {
-                    let s = Wi(o),
-                        u = K0(n, s),
-                        f = B.makeSpan(["katex"], [u]);
-                    return Yi(f, o)
+                        let p = Qi(n, t, s, o.displayMode, !1),
+                            b = en(n, s);
+                        u = B.makeSpan(["katex"], [p, b])
+                    }
+                    return Ji(u, o)
+                },
+                m1 = function(n, t, o) {
+                    let s = Xi(o),
+                        u = en(n, s),
+                        p = B.makeSpan(["katex"], [u]);
+                    return Ji(p, o)
                 };
-            var jp = null;
-            let m1 = {
+            var Xp = null;
+            let p1 = {
                     widehat: "^",
                     widecheck: "\u02C7",
                     widetilde: "~",
                     utilde: "~",
                     overleftarrow: "\u2190",
                     underleftarrow: "\u2190",
                     xleftarrow: "\u2190",
@@ -9910,19 +9910,19 @@
                     xrightleftarrows: "\u21C4",
                     xrightequilibrium: "\u21CC",
                     xleftequilibrium: "\u21CB",
                     "\\cdrightarrow": "\u2192",
                     "\\cdleftarrow": "\u2190",
                     "\\cdlongequal": "="
                 },
-                p1 = function(n) {
-                    let t = new V.MathNode("mo", [new V.TextNode(m1[n.replace(/^\\/, "")])]);
+                f1 = function(n) {
+                    let t = new V.MathNode("mo", [new V.TextNode(p1[n.replace(/^\\/, "")])]);
                     return t.setAttribute("stretchy", "true"), t
                 },
-                f1 = {
+                g1 = {
                     overrightarrow: [
                         ["rightarrow"], .888, 522, "xMaxYMin"
                     ],
                     overleftarrow: [
                         ["leftarrow"], .888, 522, "xMinYMin"
                     ],
                     underrightarrow: [
@@ -10036,216 +10036,216 @@
                     xrightequilibrium: [
                         ["baraboveshortleftharpoon", "rightharpoonaboveshortbar"], 1.75, 716
                     ],
                     xleftequilibrium: [
                         ["shortbaraboveleftharpoon", "shortrightharpoonabovebar"], 1.75, 716
                     ]
                 },
-                g1 = function(n) {
+                b1 = function(n) {
                     return n.type === "ordgroup" ? n.body.length : 1
                 };
             var Ft = {
                 encloseSpan: function(n, t, o, s, u) {
-                    let f, b = n.height + n.depth + o + s;
+                    let p, b = n.height + n.depth + o + s;
                     if (/fbox|color|angl/.test(t)) {
-                        if (f = B.makeSpan(["stretchy", t], [], u), t === "fbox") {
+                        if (p = B.makeSpan(["stretchy", t], [], u), t === "fbox") {
                             let v = u.color && u.getColor();
-                            v && (f.style.borderColor = v)
+                            v && (p.style.borderColor = v)
                         }
                     } else {
                         let v = [];
-                        /^[bx]cancel$/.test(t) && v.push(new W0({
+                        /^[bx]cancel$/.test(t) && v.push(new Y0({
                             x1: "0",
                             y1: "0",
                             x2: "100%",
                             y2: "100%",
                             "stroke-width": "0.046em"
-                        })), /^x?cancel$/.test(t) && v.push(new W0({
+                        })), /^x?cancel$/.test(t) && v.push(new Y0({
                             x1: "0",
                             y1: "100%",
                             x2: "100%",
                             y2: "0",
                             "stroke-width": "0.046em"
                         }));
                         let S = new Et(v, {
                             width: "100%",
-                            height: Q(b)
+                            height: Z(b)
                         });
-                        f = B.makeSvgSpan([], [S], u)
+                        p = B.makeSvgSpan([], [S], u)
                     }
-                    return f.height = b, f.style.height = Q(b), f
+                    return p.height = b, p.style.height = Z(b), p
                 },
-                mathMLnode: p1,
+                mathMLnode: f1,
                 svgSpan: function(n, t) {
                     function o() {
                         let b = 4e5,
                             v = n.label.slice(1);
                         if (R.contains(["widehat", "widecheck", "widetilde", "utilde"], v)) {
-                            let E = g1(n.base),
+                            let E = b1(n.base),
                                 z, F, N;
                             if (E > 5) v === "widehat" || v === "widecheck" ? (z = 420, b = 2364, N = .42, F = v + "4") : (z = 312, b = 2340, N = .34, F = "tilde4");
                             else {
                                 let ie = [1, 1, 2, 2, 3, 3][E];
                                 v === "widehat" || v === "widecheck" ? (b = [0, 1062, 2364, 2364, 2364][ie], z = [0, 239, 300, 360, 420][ie], N = [0, .24, .3, .3, .36, .42][ie], F = v + ie) : (b = [0, 600, 1033, 2339, 2340][ie], z = [0, 260, 286, 306, 312][ie], N = [0, .26, .286, .3, .306, .34][ie], F = "tilde" + ie)
                             }
-                            let O = new Ot(F),
-                                K = new Et([O], {
+                            let H = new Ot(F),
+                                K = new Et([H], {
                                     width: "100%",
-                                    height: Q(N),
+                                    height: Z(N),
                                     viewBox: "0 0 " + b + " " + z,
                                     preserveAspectRatio: "none"
                                 });
                             return {
                                 span: B.makeSvgSpan([], [K], t),
                                 minWidth: 0,
                                 height: N
                             }
                         } else {
                             let S = [],
-                                E = f1[v],
+                                E = g1[v],
                                 [z, F, N] = E,
-                                O = N / 1e3,
+                                H = N / 1e3,
                                 K = z.length,
                                 ie, ye;
                             if (K === 1) {
                                 let ge = E[3];
                                 ie = ["hide-tail"], ye = [ge]
                             } else if (K === 2) ie = ["halfarrow-left", "halfarrow-right"], ye = ["xMinYMin", "xMaxYMin"];
                             else if (K === 3) ie = ["brace-left", "brace-center", "brace-right"], ye = ["xMinYMin", "xMidYMin", "xMaxYMin"];
                             else throw new Error(`Correct katexImagesData or update code here to support
                     ` + K + " children.");
                             for (let ge = 0; ge < K; ge++) {
                                 let xe = new Ot(z[ge]),
                                     ke = new Et([xe], {
                                         width: "400em",
-                                        height: Q(O),
+                                        height: Z(H),
                                         viewBox: "0 0 " + b + " " + N,
                                         preserveAspectRatio: ye[ge] + " slice"
                                     }),
                                     ze = B.makeSvgSpan([ie[ge]], [ke], t);
                                 if (K === 1) return {
                                     span: ze,
                                     minWidth: F,
-                                    height: O
+                                    height: H
                                 };
-                                ze.style.height = Q(O), S.push(ze)
+                                ze.style.height = Z(H), S.push(ze)
                             }
                             return {
                                 span: B.makeSpan(["stretchy"], S, t),
                                 minWidth: F,
-                                height: O
+                                height: H
                             }
                         }
                     }
                     let {
                         span: s,
                         minWidth: u,
-                        height: f
+                        height: p
                     } = o();
-                    return s.height = f, s.style.height = Q(f), u > 0 && (s.style.minWidth = Q(u)), s
+                    return s.height = p, s.style.height = Z(p), u > 0 && (s.style.minWidth = Z(u)), s
                 }
             };
 
             function de(n, t) {
                 if (!n || n.type !== t) throw new Error("Expected node of type " + t + ", but got " + (n ? "node of type " + n.type : String(n)));
                 return n
             }
 
-            function rn(n) {
-                let t = Jr(n);
+            function nn(n) {
+                let t = Kr(n);
                 if (!t) throw new Error("Expected node of symbol group type, but got " + (n ? "node of type " + n.type : String(n)));
                 return t
             }
 
-            function Jr(n) {
-                return n && (n.type === "atom" || ju.hasOwnProperty(n.type)) ? n : null
+            function Kr(n) {
+                return n && (n.type === "atom" || Uu.hasOwnProperty(n.type)) ? n : null
             }
-            let nn = (n, t) => {
+            let on = (n, t) => {
                     let o, s, u;
-                    n && n.type === "supsub" ? (s = de(n.base, "accent"), o = s.base, n.base = o, u = Gu(ve(n, t)), n.base = s) : (s = de(n, "accent"), o = s.base);
-                    let f = ve(o, t.havingCrampedStyle()),
+                    n && n.type === "supsub" ? (s = de(n.base, "accent"), o = s.base, n.base = o, u = Vu(ve(n, t)), n.base = s) : (s = de(n, "accent"), o = s.base);
+                    let p = ve(o, t.havingCrampedStyle()),
                         b = s.isShifty && R.isCharacterBox(o),
                         v = 0;
                     if (b) {
                         let N = R.getBaseElem(o),
-                            O = ve(N, t.havingCrampedStyle());
-                        v = Fi(O).skew
+                            H = ve(N, t.havingCrampedStyle());
+                        v = Pi(H).skew
                     }
                     let S = s.label === "\\c",
-                        E = S ? f.height + f.depth : Math.min(f.height, t.fontMetrics().xHeight),
+                        E = S ? p.height + p.depth : Math.min(p.height, t.fontMetrics().xHeight),
                         z;
                     if (s.isStretchy) z = Ft.svgSpan(s, t), z = B.makeVList({
                         positionType: "firstBaseline",
                         children: [{
                             type: "elem",
-                            elem: f
+                            elem: p
                         }, {
                             type: "elem",
                             elem: z,
                             wrapperClasses: ["svg-align"],
                             wrapperStyle: v > 0 ? {
-                                width: "calc(100% - " + Q(2 * v) + ")",
-                                marginLeft: Q(2 * v)
+                                width: "calc(100% - " + Z(2 * v) + ")",
+                                marginLeft: Z(2 * v)
                             } : void 0
                         }]
                     }, t);
                     else {
-                        let N, O;
-                        s.label === "\\vec" ? (N = B.staticSvg("vec", t), O = B.svgData.vec[1]) : (N = B.makeOrd({
+                        let N, H;
+                        s.label === "\\vec" ? (N = B.staticSvg("vec", t), H = B.svgData.vec[1]) : (N = B.makeOrd({
                             mode: s.mode,
                             text: s.label
-                        }, t, "textord"), N = Fi(N), N.italic = 0, O = N.width, S && (E += N.depth)), z = B.makeSpan(["accent-body"], [N]);
+                        }, t, "textord"), N = Pi(N), N.italic = 0, H = N.width, S && (E += N.depth)), z = B.makeSpan(["accent-body"], [N]);
                         let K = s.label === "\\textcircled";
-                        K && (z.classes.push("accent-full"), E = f.height);
+                        K && (z.classes.push("accent-full"), E = p.height);
                         let ie = v;
-                        K || (ie -= O / 2), z.style.left = Q(ie), s.label === "\\textcircled" && (z.style.top = ".2em"), z = B.makeVList({
+                        K || (ie -= H / 2), z.style.left = Z(ie), s.label === "\\textcircled" && (z.style.top = ".2em"), z = B.makeVList({
                             positionType: "firstBaseline",
                             children: [{
                                 type: "elem",
-                                elem: f
+                                elem: p
                             }, {
                                 type: "kern",
                                 size: -E
                             }, {
                                 type: "elem",
                                 elem: z
                             }]
                         }, t)
                     }
                     let F = B.makeSpan(["mord", "accent"], [z], t);
                     return u ? (u.children[0] = F, u.height = Math.max(F.height, u.height), u.classes[0] = "mord", u) : F
                 },
-                Qi = (n, t) => {
+                Ki = (n, t) => {
                     let o = n.isStretchy ? Ft.mathMLnode(n.label) : new V.MathNode("mo", [dt(n.label, n.mode)]),
                         s = new V.MathNode("mover", [Ee(n.base, t), o]);
                     return s.setAttribute("accent", "true"), s
                 },
-                b1 = new RegExp(["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring"].map(n => "\\" + n).join("|"));
-            Z({
+                y1 = new RegExp(["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring"].map(n => "\\" + n).join("|"));
+            Q({
                 type: "accent",
                 names: ["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring", "\\widecheck", "\\widehat", "\\widetilde", "\\overrightarrow", "\\overleftarrow", "\\Overrightarrow", "\\overleftrightarrow", "\\overgroup", "\\overlinesegment", "\\overleftharpoon", "\\overrightharpoon"],
                 props: {
                     numArgs: 1
                 },
                 handler: (n, t) => {
-                    let o = Zr(t[0]),
-                        s = !b1.test(n.funcName),
+                    let o = Xr(t[0]),
+                        s = !y1.test(n.funcName),
                         u = !s || n.funcName === "\\widehat" || n.funcName === "\\widetilde" || n.funcName === "\\widecheck";
                     return {
                         type: "accent",
                         mode: n.parser.mode,
                         label: n.funcName,
                         isStretchy: s,
                         isShifty: u,
                         base: o
                     }
                 },
-                htmlBuilder: nn,
-                mathmlBuilder: Qi
-            }), Z({
+                htmlBuilder: on,
+                mathmlBuilder: Ki
+            }), Q({
                 type: "accent",
                 names: ["\\'", "\\`", "\\^", "\\~", "\\=", "\\u", "\\.", '\\"', "\\c", "\\r", "\\H", "\\v", "\\textcircled"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0,
                     allowedInMath: !0,
                     argTypes: ["primitive"]
@@ -10258,17 +10258,17 @@
                         mode: s,
                         label: n.funcName,
                         isStretchy: !1,
                         isShifty: !0,
                         base: o
                     }
                 },
-                htmlBuilder: nn,
-                mathmlBuilder: Qi
-            }), Z({
+                htmlBuilder: on,
+                mathmlBuilder: Ki
+            }), Q({
                 type: "accentUnder",
                 names: ["\\underleftarrow", "\\underrightarrow", "\\underleftrightarrow", "\\undergroup", "\\underlinesegment", "\\utilde"],
                 props: {
                     numArgs: 1
                 },
                 handler: (n, t) => {
                     let {
@@ -10282,42 +10282,42 @@
                         base: u
                     }
                 },
                 htmlBuilder: (n, t) => {
                     let o = ve(n.base, t),
                         s = Ft.svgSpan(n, t),
                         u = n.label === "\\utilde" ? .12 : 0,
-                        f = B.makeVList({
+                        p = B.makeVList({
                             positionType: "top",
                             positionData: o.height,
                             children: [{
                                 type: "elem",
                                 elem: s,
                                 wrapperClasses: ["svg-align"]
                             }, {
                                 type: "kern",
                                 size: u
                             }, {
                                 type: "elem",
                                 elem: o
                             }]
                         }, t);
-                    return B.makeSpan(["mord", "accentunder"], [f], t)
+                    return B.makeSpan(["mord", "accentunder"], [p], t)
                 },
                 mathmlBuilder: (n, t) => {
                     let o = Ft.mathMLnode(n.label),
                         s = new V.MathNode("munder", [Ee(n.base, t), o]);
                     return s.setAttribute("accentunder", "true"), s
                 }
             });
-            let Kr = n => {
+            let e0 = n => {
                 let t = new V.MathNode("mpadded", n ? [n] : []);
                 return t.setAttribute("width", "+0.6em"), t.setAttribute("lspace", "0.3em"), t
             };
-            Z({
+            Q({
                 type: "xArrow",
                 names: ["\\xleftarrow", "\\xrightarrow", "\\xLeftarrow", "\\xRightarrow", "\\xleftrightarrow", "\\xLeftrightarrow", "\\xhookleftarrow", "\\xhookrightarrow", "\\xmapsto", "\\xrightharpoondown", "\\xrightharpoonup", "\\xleftharpoondown", "\\xleftharpoonup", "\\xrightleftharpoons", "\\xleftrightharpoons", "\\xlongequal", "\\xtwoheadrightarrow", "\\xtwoheadleftarrow", "\\xtofrom", "\\xrightleftarrows", "\\xrightequilibrium", "\\xleftequilibrium", "\\\\cdrightarrow", "\\\\cdleftarrow", "\\\\cdlongequal"],
                 props: {
                     numArgs: 1,
                     numOptionalArgs: 1
                 },
                 handler(n, t, o) {
@@ -10333,18 +10333,18 @@
                         below: o[0]
                     }
                 },
                 htmlBuilder(n, t) {
                     let o = t.style,
                         s = t.havingStyle(o.sup()),
                         u = B.wrapFragment(ve(n.body, s, t), t),
-                        f = n.label.slice(0, 2) === "\\x" ? "x" : "cd";
-                    u.classes.push(f + "-arrow-pad");
+                        p = n.label.slice(0, 2) === "\\x" ? "x" : "cd";
+                    u.classes.push(p + "-arrow-pad");
                     let b;
-                    n.below && (s = t.havingStyle(o.sub()), b = B.wrapFragment(ve(n.below, s, t), t), b.classes.push(f + "-arrow-pad"));
+                    n.below && (s = t.havingStyle(o.sub()), b = B.wrapFragment(ve(n.below, s, t), t), b.classes.push(p + "-arrow-pad"));
                     let v = Ft.svgSpan(n, t),
                         S = -t.fontMetrics().axisHeight + .5 * v.height,
                         E = -t.fontMetrics().axisHeight - .5 * v.height - .111;
                     (u.depth > .25 || n.label === "\\xleftequilibrium") && (E -= u.depth);
                     let z;
                     if (b) {
                         let F = -t.fontMetrics().axisHeight + b.height + .5 * v.height + .111;
@@ -10379,38 +10379,38 @@
                     return z.children[0].children[0].children[1].classes.push("svg-align"), B.makeSpan(["mrel", "x-arrow"], [z], t)
                 },
                 mathmlBuilder(n, t) {
                     let o = Ft.mathMLnode(n.label);
                     o.setAttribute("minsize", n.label.charAt(0) === "x" ? "1.75em" : "3.0em");
                     let s;
                     if (n.body) {
-                        let u = Kr(Ee(n.body, t));
+                        let u = e0(Ee(n.body, t));
                         if (n.below) {
-                            let f = Kr(Ee(n.below, t));
-                            s = new V.MathNode("munderover", [o, f, u])
+                            let p = e0(Ee(n.below, t));
+                            s = new V.MathNode("munderover", [o, p, u])
                         } else s = new V.MathNode("mover", [o, u])
                     } else if (n.below) {
-                        let u = Kr(Ee(n.below, t));
+                        let u = e0(Ee(n.below, t));
                         s = new V.MathNode("munder", [o, u])
-                    } else s = Kr(), s = new V.MathNode("mover", [o, s]);
+                    } else s = e0(), s = new V.MathNode("mover", [o, s]);
                     return s
                 }
             });
-            let y1 = B.makeSpan;
+            let x1 = B.makeSpan;
 
-            function Zi(n, t) {
-                let o = Qe(n.body, t, !0);
-                return y1([n.mclass], o, t)
+            function eo(n, t) {
+                let o = Ze(n.body, t, !0);
+                return x1([n.mclass], o, t)
             }
 
-            function Xi(n, t) {
+            function to(n, t) {
                 let o, s = it(n.body, t);
                 return n.mclass === "minner" ? o = new V.MathNode("mpadded", s) : n.mclass === "mord" ? n.isCharacterBox ? (o = s[0], o.type = "mi") : o = new V.MathNode("mi", s) : (n.isCharacterBox ? (o = s[0], o.type = "mo") : o = new V.MathNode("mo", s), n.mclass === "mbin" ? (o.attributes.lspace = "0.22em", o.attributes.rspace = "0.22em") : n.mclass === "mpunct" ? (o.attributes.lspace = "0em", o.attributes.rspace = "0.17em") : n.mclass === "mopen" || n.mclass === "mclose" ? (o.attributes.lspace = "0em", o.attributes.rspace = "0em") : n.mclass === "minner" && (o.attributes.lspace = "0.0556em", o.attributes.width = "+0.1111em")), o
             }
-            Z({
+            Q({
                 type: "mclass",
                 names: ["\\mathord", "\\mathbin", "\\mathrel", "\\mathopen", "\\mathclose", "\\mathpunct", "\\mathinner"],
                 props: {
                     numArgs: 1,
                     primitive: !0
                 },
                 handler(n, t) {
@@ -10422,141 +10422,141 @@
                         type: "mclass",
                         mode: o.mode,
                         mclass: "m" + s.slice(5),
                         body: je(u),
                         isCharacterBox: R.isCharacterBox(u)
                     }
                 },
-                htmlBuilder: Zi,
-                mathmlBuilder: Xi
+                htmlBuilder: eo,
+                mathmlBuilder: to
             });
-            let e0 = n => {
+            let t0 = n => {
                 let t = n.type === "ordgroup" && n.body.length ? n.body[0] : n;
                 return t.type === "atom" && (t.family === "bin" || t.family === "rel") ? "m" + t.family : "mord"
             };
-            Z({
+            Q({
                 type: "mclass",
                 names: ["\\@binrel"],
                 props: {
                     numArgs: 2
                 },
                 handler(n, t) {
                     let {
                         parser: o
                     } = n;
                     return {
                         type: "mclass",
                         mode: o.mode,
-                        mclass: e0(t[0]),
+                        mclass: t0(t[0]),
                         body: je(t[1]),
                         isCharacterBox: R.isCharacterBox(t[1])
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "mclass",
                 names: ["\\stackrel", "\\overset", "\\underset"],
                 props: {
                     numArgs: 2
                 },
                 handler(n, t) {
                     let {
                         parser: o,
                         funcName: s
-                    } = n, u = t[1], f = t[0], b;
-                    s !== "\\stackrel" ? b = e0(u) : b = "mrel";
+                    } = n, u = t[1], p = t[0], b;
+                    s !== "\\stackrel" ? b = t0(u) : b = "mrel";
                     let v = {
                             type: "op",
                             mode: u.mode,
                             limits: !0,
                             alwaysHandleSupSub: !0,
                             parentIsSupSub: !1,
                             symbol: !1,
                             suppressBaseShift: s !== "\\stackrel",
                             body: je(u)
                         },
                         S = {
                             type: "supsub",
-                            mode: f.mode,
+                            mode: p.mode,
                             base: v,
-                            sup: s === "\\underset" ? null : f,
-                            sub: s === "\\underset" ? f : null
+                            sup: s === "\\underset" ? null : p,
+                            sub: s === "\\underset" ? p : null
                         };
                     return {
                         type: "mclass",
                         mode: o.mode,
                         mclass: b,
                         body: [S],
                         isCharacterBox: R.isCharacterBox(S)
                     }
                 },
-                htmlBuilder: Zi,
-                mathmlBuilder: Xi
-            }), Z({
+                htmlBuilder: eo,
+                mathmlBuilder: to
+            }), Q({
                 type: "pmb",
                 names: ["\\pmb"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0
                 },
                 handler(n, t) {
                     let {
                         parser: o
                     } = n;
                     return {
                         type: "pmb",
                         mode: o.mode,
-                        mclass: e0(t[0]),
+                        mclass: t0(t[0]),
                         body: je(t[0])
                     }
                 },
                 htmlBuilder(n, t) {
-                    let o = Qe(n.body, t, !0),
+                    let o = Ze(n.body, t, !0),
                         s = B.makeSpan([n.mclass], o, t);
                     return s.style.textShadow = "0.02em 0.01em 0.04px", s
                 },
                 mathmlBuilder(n, t) {
                     let o = it(n.body, t),
                         s = new V.MathNode("mstyle", o);
                     return s.setAttribute("style", "text-shadow: 0.02em 0.01em 0.04px"), s
                 }
             });
-            let x1 = {
+            let v1 = {
                     ">": "\\\\cdrightarrow",
                     "<": "\\\\cdleftarrow",
                     "=": "\\\\cdlongequal",
                     A: "\\uparrow",
                     V: "\\downarrow",
                     "|": "\\Vert",
                     ".": "no arrow"
                 },
-                Ji = () => ({
+                ro = () => ({
                     type: "styling",
                     body: [],
                     mode: "math",
                     style: "display"
                 }),
-                Ki = n => n.type === "textord" && n.text === "@",
-                v1 = (n, t) => (n.type === "mathord" || n.type === "atom") && n.text === t;
+                no = n => n.type === "textord" && n.text === "@",
+                w1 = (n, t) => (n.type === "mathord" || n.type === "atom") && n.text === t;
 
-            function w1(n, t, o) {
-                let s = x1[n];
+            function k1(n, t, o) {
+                let s = v1[n];
                 switch (s) {
                     case "\\\\cdrightarrow":
                     case "\\\\cdleftarrow":
                         return o.callFunction(s, [t[0]], [t[1]]);
                     case "\\uparrow":
                     case "\\downarrow": {
                         let u = o.callFunction("\\\\cdleft", [t[0]], []),
-                            f = {
+                            p = {
                                 type: "atom",
                                 text: s,
                                 mode: "math",
                                 family: "rel"
                             },
-                            b = o.callFunction("\\Big", [f], []),
+                            b = o.callFunction("\\Big", [p], []),
                             v = o.callFunction("\\\\cdright", [t[1]], []),
                             S = {
                                 type: "ordgroup",
                                 mode: "math",
                                 body: [u, b, v]
                             };
                         return o.callFunction("\\\\cdparent", [S], [])
@@ -10574,66 +10574,66 @@
                     default:
                         return {
                             type: "textord", text: " ", mode: "math"
                         }
                 }
             }
 
-            function k1(n) {
+            function _1(n) {
                 let t = [];
                 for (n.gullet.beginGroup(), n.gullet.macros.set("\\cr", "\\\\\\relax"), n.gullet.beginGroup();;) {
                     t.push(n.parseExpression(!1, "\\\\")), n.gullet.endGroup(), n.gullet.beginGroup();
-                    let f = n.fetch().text;
-                    if (f === "&" || f === "\\\\") n.consume();
-                    else if (f === "\\end") {
+                    let p = n.fetch().text;
+                    if (p === "&" || p === "\\\\") n.consume();
+                    else if (p === "\\end") {
                         t[t.length - 1].length === 0 && t.pop();
                         break
                     } else throw new a("Expected \\\\ or \\cr or \\end", n.nextToken)
                 }
                 let o = [],
                     s = [o];
-                for (let f = 0; f < t.length; f++) {
-                    let b = t[f],
-                        v = Ji();
+                for (let p = 0; p < t.length; p++) {
+                    let b = t[p],
+                        v = ro();
                     for (let S = 0; S < b.length; S++)
-                        if (!Ki(b[S])) v.body.push(b[S]);
+                        if (!no(b[S])) v.body.push(b[S]);
                         else {
                             o.push(v), S += 1;
-                            let E = rn(b[S]).text,
+                            let E = nn(b[S]).text,
                                 z = new Array(2);
                             if (z[0] = {
                                     type: "ordgroup",
                                     mode: "math",
                                     body: []
                                 }, z[1] = {
                                     type: "ordgroup",
                                     mode: "math",
                                     body: []
                                 }, !("=|.".indexOf(E) > -1))
                                 if ("<>AV".indexOf(E) > -1)
-                                    for (let O = 0; O < 2; O++) {
+                                    for (let H = 0; H < 2; H++) {
                                         let K = !0;
                                         for (let ie = S + 1; ie < b.length; ie++) {
-                                            if (v1(b[ie], E)) {
+                                            if (w1(b[ie], E)) {
                                                 K = !1, S = ie;
                                                 break
                                             }
-                                            if (Ki(b[ie])) throw new a("Missing a " + E + " character to complete a CD arrow.", b[ie]);
-                                            z[O].body.push(b[ie])
+                                            if (no(b[ie])) throw new a("Missing a " + E + " character to complete a CD arrow.", b[ie]);
+                                            z[H].body.push(b[ie])
                                         }
                                         if (K) throw new a("Missing a " + E + " character to complete a CD arrow.", b[S])
                                     } else throw new a('Expected one of "<>AV=|." after @', b[S]);
                             let N = {
                                 type: "styling",
-                                body: [w1(E, z, n)],
+                                body: [k1(E, z, n)],
                                 mode: "math",
                                 style: "display"
                             };
-                            o.push(N), v = Ji()
-                        } f % 2 === 0 ? o.push(v) : o.shift(), o = [], s.push(o)
+                            o.push(N), v = ro()
+                        } p % 2 === 0 ? o.push(v) : o.shift(), o = [], s.push(o)
                 }
                 n.gullet.endGroup(), n.gullet.endGroup();
                 let u = new Array(s[0].length).fill({
                     type: "align",
                     align: "c",
                     pregap: .25,
                     postgap: .25
@@ -10646,15 +10646,15 @@
                     addJot: !0,
                     rowGaps: [null],
                     cols: u,
                     colSeparationType: "CD",
                     hLinesBeforeRow: new Array(s.length + 1).fill([])
                 }
             }
-            Z({
+            Q({
                 type: "cdlabel",
                 names: ["\\\\cdleft", "\\\\cdright"],
                 props: {
                     numArgs: 1
                 },
                 handler(n, t) {
                     let {
@@ -10667,21 +10667,21 @@
                         side: s.slice(4),
                         label: t[0]
                     }
                 },
                 htmlBuilder(n, t) {
                     let o = t.havingStyle(t.style.sup()),
                         s = B.wrapFragment(ve(n.label, o, t), t);
-                    return s.classes.push("cd-label-" + n.side), s.style.bottom = Q(.8 - s.depth), s.height = 0, s.depth = 0, s
+                    return s.classes.push("cd-label-" + n.side), s.style.bottom = Z(.8 - s.depth), s.height = 0, s.depth = 0, s
                 },
                 mathmlBuilder(n, t) {
                     let o = new V.MathNode("mrow", [Ee(n.label, t)]);
                     return o = new V.MathNode("mpadded", [o]), o.setAttribute("width", "0"), n.side === "left" && o.setAttribute("lspace", "-1width"), o.setAttribute("voffset", "0.7em"), o = new V.MathNode("mstyle", [o]), o.setAttribute("displaystyle", "false"), o.setAttribute("scriptlevel", "1"), o
                 }
-            }), Z({
+            }), Q({
                 type: "cdlabelparent",
                 names: ["\\\\cdparent"],
                 props: {
                     numArgs: 1
                 },
                 handler(n, t) {
                     let {
@@ -10696,50 +10696,50 @@
                 htmlBuilder(n, t) {
                     let o = B.wrapFragment(ve(n.fragment, t), t);
                     return o.classes.push("cd-vert-arrow"), o
                 },
                 mathmlBuilder(n, t) {
                     return new V.MathNode("mrow", [Ee(n.fragment, t)])
                 }
-            }), Z({
+            }), Q({
                 type: "textord",
                 names: ["\\@char"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0
                 },
                 handler(n, t) {
                     let {
                         parser: o
-                    } = n, u = de(t[0], "ordgroup").body, f = "";
+                    } = n, u = de(t[0], "ordgroup").body, p = "";
                     for (let S = 0; S < u.length; S++) {
                         let E = de(u[S], "textord");
-                        f += E.text
+                        p += E.text
                     }
-                    let b = parseInt(f),
+                    let b = parseInt(p),
                         v;
-                    if (isNaN(b)) throw new a("\\@char has non-numeric argument " + f);
-                    if (b < 0 || b >= 1114111) throw new a("\\@char with invalid code point " + f);
+                    if (isNaN(b)) throw new a("\\@char has non-numeric argument " + p);
+                    if (b < 0 || b >= 1114111) throw new a("\\@char with invalid code point " + p);
                     return b <= 65535 ? v = String.fromCharCode(b) : (b -= 65536, v = String.fromCharCode((b >> 10) + 55296, (b & 1023) + 56320)), {
                         type: "textord",
                         mode: o.mode,
                         text: v
                     }
                 }
             });
-            let eo = (n, t) => {
-                    let o = Qe(n.body, t.withColor(n.color), !1);
+            let io = (n, t) => {
+                    let o = Ze(n.body, t.withColor(n.color), !1);
                     return B.makeFragment(o)
                 },
-                to = (n, t) => {
+                oo = (n, t) => {
                     let o = it(n.body, t.withColor(n.color)),
                         s = new V.MathNode("mstyle", o);
                     return s.setAttribute("mathcolor", n.color), s
                 };
-            Z({
+            Q({
                 type: "color",
                 names: ["\\textcolor"],
                 props: {
                     numArgs: 2,
                     allowedInText: !0,
                     argTypes: ["color", "original"]
                 },
@@ -10750,394 +10750,394 @@
                     return {
                         type: "color",
                         mode: o.mode,
                         color: s,
                         body: je(u)
                     }
                 },
-                htmlBuilder: eo,
-                mathmlBuilder: to
-            }), Z({
+                htmlBuilder: io,
+                mathmlBuilder: oo
+            }), Q({
                 type: "color",
                 names: ["\\color"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0,
                     argTypes: ["color"]
                 },
                 handler(n, t) {
                     let {
                         parser: o,
                         breakOnTokenText: s
                     } = n, u = de(t[0], "color-token").color;
                     o.gullet.macros.set("\\current@color", u);
-                    let f = o.parseExpression(!0, s);
+                    let p = o.parseExpression(!0, s);
                     return {
                         type: "color",
                         mode: o.mode,
                         color: u,
-                        body: f
+                        body: p
                     }
                 },
-                htmlBuilder: eo,
-                mathmlBuilder: to
-            }), Z({
+                htmlBuilder: io,
+                mathmlBuilder: oo
+            }), Q({
                 type: "cr",
                 names: ["\\\\"],
                 props: {
                     numArgs: 0,
                     numOptionalArgs: 0,
                     allowedInText: !0
                 },
                 handler(n, t, o) {
                     let {
                         parser: s
-                    } = n, u = s.gullet.future().text === "[" ? s.parseSizeGroup(!0) : null, f = !s.settings.displayMode || !s.settings.useStrictBehavior("newLineInDisplayMode", "In LaTeX, \\\\ or \\newline does nothing in display mode");
+                    } = n, u = s.gullet.future().text === "[" ? s.parseSizeGroup(!0) : null, p = !s.settings.displayMode || !s.settings.useStrictBehavior("newLineInDisplayMode", "In LaTeX, \\\\ or \\newline does nothing in display mode");
                     return {
                         type: "cr",
                         mode: s.mode,
-                        newLine: f,
+                        newLine: p,
                         size: u && de(u, "size").value
                     }
                 },
                 htmlBuilder(n, t) {
                     let o = B.makeSpan(["mspace"], [], t);
-                    return n.newLine && (o.classes.push("newline"), n.size && (o.style.marginTop = Q(Ie(n.size, t)))), o
+                    return n.newLine && (o.classes.push("newline"), n.size && (o.style.marginTop = Z(Ie(n.size, t)))), o
                 },
                 mathmlBuilder(n, t) {
                     let o = new V.MathNode("mspace");
-                    return n.newLine && (o.setAttribute("linebreak", "newline"), n.size && o.setAttribute("height", Q(Ie(n.size, t)))), o
+                    return n.newLine && (o.setAttribute("linebreak", "newline"), n.size && o.setAttribute("height", Z(Ie(n.size, t)))), o
                 }
             });
-            let on = {
+            let an = {
                     "\\global": "\\global",
                     "\\long": "\\\\globallong",
                     "\\\\globallong": "\\\\globallong",
                     "\\def": "\\gdef",
                     "\\gdef": "\\gdef",
                     "\\edef": "\\xdef",
                     "\\xdef": "\\xdef",
                     "\\let": "\\\\globallet",
                     "\\futurelet": "\\\\globalfuture"
                 },
-                ro = n => {
+                ao = n => {
                     let t = n.text;
                     if (/^(?:[\\{}$&#^_]|EOF)$/.test(t)) throw new a("Expected a control sequence", n);
                     return t
                 },
-                _1 = n => {
+                S1 = n => {
                     let t = n.gullet.popToken();
                     return t.text === "=" && (t = n.gullet.popToken(), t.text === " " && (t = n.gullet.popToken())), t
                 },
-                no = (n, t, o, s) => {
+                so = (n, t, o, s) => {
                     let u = n.gullet.macros.get(o.text);
                     u == null && (o.noexpand = !0, u = {
                         tokens: [o],
                         numArgs: 0,
                         unexpandable: !n.gullet.isExpandable(o.text)
                     }), n.gullet.macros.set(t, u, s)
                 };
-            Z({
+            Q({
                 type: "internal",
                 names: ["\\global", "\\long", "\\\\globallong"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0
                 },
                 handler(n) {
                     let {
                         parser: t,
                         funcName: o
                     } = n;
                     t.consumeSpaces();
                     let s = t.fetch();
-                    if (on[s.text]) return (o === "\\global" || o === "\\\\globallong") && (s.text = on[s.text]), de(t.parseFunction(), "internal");
+                    if (an[s.text]) return (o === "\\global" || o === "\\\\globallong") && (s.text = an[s.text]), de(t.parseFunction(), "internal");
                     throw new a("Invalid token after macro prefix", s)
                 }
-            }), Z({
+            }), Q({
                 type: "internal",
                 names: ["\\def", "\\gdef", "\\edef", "\\xdef"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0,
                     primitive: !0
                 },
                 handler(n) {
                     let {
                         parser: t,
                         funcName: o
                     } = n, s = t.gullet.popToken(), u = s.text;
                     if (/^(?:[\\{}$&#^_]|EOF)$/.test(u)) throw new a("Expected a control sequence", s);
-                    let f = 0,
+                    let p = 0,
                         b, v = [
                             []
                         ];
                     for (; t.gullet.future().text !== "{";)
                         if (s = t.gullet.popToken(), s.text === "#") {
                             if (t.gullet.future().text === "{") {
-                                b = t.gullet.future(), v[f].push("{");
+                                b = t.gullet.future(), v[p].push("{");
                                 break
                             }
                             if (s = t.gullet.popToken(), !/^[1-9]$/.test(s.text)) throw new a('Invalid argument number "' + s.text + '"');
-                            if (parseInt(s.text) !== f + 1) throw new a('Argument number "' + s.text + '" out of order');
-                            f++, v.push([])
+                            if (parseInt(s.text) !== p + 1) throw new a('Argument number "' + s.text + '" out of order');
+                            p++, v.push([])
                         } else {
                             if (s.text === "EOF") throw new a("Expected a macro definition");
-                            v[f].push(s.text)
+                            v[p].push(s.text)
                         } let {
                         tokens: S
                     } = t.gullet.consumeArg();
                     return b && S.unshift(b), (o === "\\edef" || o === "\\xdef") && (S = t.gullet.expandTokens(S), S.reverse()), t.gullet.macros.set(u, {
                         tokens: S,
-                        numArgs: f,
+                        numArgs: p,
                         delimiters: v
-                    }, o === on[o]), {
+                    }, o === an[o]), {
                         type: "internal",
                         mode: t.mode
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "internal",
                 names: ["\\let", "\\\\globallet"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0,
                     primitive: !0
                 },
                 handler(n) {
                     let {
                         parser: t,
                         funcName: o
-                    } = n, s = ro(t.gullet.popToken());
+                    } = n, s = ao(t.gullet.popToken());
                     t.gullet.consumeSpaces();
-                    let u = _1(t);
-                    return no(t, s, u, o === "\\\\globallet"), {
+                    let u = S1(t);
+                    return so(t, s, u, o === "\\\\globallet"), {
                         type: "internal",
                         mode: t.mode
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "internal",
                 names: ["\\futurelet", "\\\\globalfuture"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0,
                     primitive: !0
                 },
                 handler(n) {
                     let {
                         parser: t,
                         funcName: o
-                    } = n, s = ro(t.gullet.popToken()), u = t.gullet.popToken(), f = t.gullet.popToken();
-                    return no(t, s, f, o === "\\\\globalfuture"), t.gullet.pushToken(f), t.gullet.pushToken(u), {
+                    } = n, s = ao(t.gullet.popToken()), u = t.gullet.popToken(), p = t.gullet.popToken();
+                    return so(t, s, p, o === "\\\\globalfuture"), t.gullet.pushToken(p), t.gullet.pushToken(u), {
                         type: "internal",
                         mode: t.mode
                     }
                 }
             });
             let _r = function(n, t, o) {
                     let s = Oe.math[n] && Oe.math[n].replace,
-                        u = G0(s || n, t, o);
+                        u = V0(s || n, t, o);
                     if (!u) throw new Error("Unsupported symbol " + n + " and font size " + t + ".");
                     return u
                 },
-                an = function(n, t, o, s) {
+                sn = function(n, t, o, s) {
                     let u = o.havingBaseStyle(t),
-                        f = B.makeSpan(s.concat(u.sizingClasses(o)), [n], o),
+                        p = B.makeSpan(s.concat(u.sizingClasses(o)), [n], o),
                         b = u.sizeMultiplier / o.sizeMultiplier;
-                    return f.height *= b, f.depth *= b, f.maxFontSize = u.sizeMultiplier, f
+                    return p.height *= b, p.depth *= b, p.maxFontSize = u.sizeMultiplier, p
                 },
-                io = function(n, t, o) {
+                lo = function(n, t, o) {
                     let s = t.havingBaseStyle(o),
                         u = (1 - t.sizeMultiplier / s.sizeMultiplier) * t.fontMetrics().axisHeight;
-                    n.classes.push("delimcenter"), n.style.top = Q(u), n.height -= u, n.depth += u
+                    n.classes.push("delimcenter"), n.style.top = Z(u), n.height -= u, n.depth += u
                 },
-                S1 = function(n, t, o, s, u, f) {
+                C1 = function(n, t, o, s, u, p) {
                     let b = B.makeSymbol(n, "Main-Regular", u, s),
-                        v = an(b, t, s, f);
-                    return o && io(v, s, t), v
+                        v = sn(b, t, s, p);
+                    return o && lo(v, s, t), v
                 },
-                C1 = function(n, t, o, s) {
+                T1 = function(n, t, o, s) {
                     return B.makeSymbol(n, "Size" + t + "-Regular", o, s)
                 },
-                oo = function(n, t, o, s, u, f) {
-                    let b = C1(n, t, u, s),
-                        v = an(B.makeSpan(["delimsizing", "size" + t], [b], s), $.TEXT, s, f);
-                    return o && io(v, s, $.TEXT), v
+                co = function(n, t, o, s, u, p) {
+                    let b = T1(n, t, u, s),
+                        v = sn(B.makeSpan(["delimsizing", "size" + t], [b], s), G.TEXT, s, p);
+                    return o && lo(v, s, G.TEXT), v
                 },
-                sn = function(n, t, o) {
+                ln = function(n, t, o) {
                     let s;
                     return t === "Size1-Regular" ? s = "delim-size1" : s = "delim-size4", {
                         type: "elem",
                         elem: B.makeSpan(["delimsizinginner", s], [B.makeSpan([], [B.makeSymbol(n, t, o)])])
                     }
                 },
-                ln = function(n, t, o) {
+                cn = function(n, t, o) {
                     let s = vt["Size4-Regular"][n.charCodeAt(0)] ? vt["Size4-Regular"][n.charCodeAt(0)][4] : vt["Size1-Regular"][n.charCodeAt(0)][4],
-                        u = new Ot("inner", Fu(n, Math.round(1e3 * t))),
-                        f = new Et([u], {
-                            width: Q(s),
-                            height: Q(t),
-                            style: "width:" + Q(s),
+                        u = new Ot("inner", Bu(n, Math.round(1e3 * t))),
+                        p = new Et([u], {
+                            width: Z(s),
+                            height: Z(t),
+                            style: "width:" + Z(s),
                             viewBox: "0 0 " + 1e3 * s + " " + Math.round(1e3 * t),
                             preserveAspectRatio: "xMinYMin"
                         }),
-                        b = B.makeSvgSpan([], [f], o);
-                    return b.height = t, b.style.height = Q(t), b.style.width = Q(s), {
+                        b = B.makeSvgSpan([], [p], o);
+                    return b.height = t, b.style.height = Z(t), b.style.width = Z(s), {
                         type: "elem",
                         elem: b
                     }
                 },
-                cn = .008,
-                t0 = {
+                un = .008,
+                r0 = {
                     type: "kern",
-                    size: -1 * cn
+                    size: -1 * un
                 },
-                T1 = ["|", "\\lvert", "\\rvert", "\\vert"],
-                A1 = ["\\|", "\\lVert", "\\rVert", "\\Vert"],
-                ao = function(n, t, o, s, u, f) {
+                A1 = ["|", "\\lvert", "\\rvert", "\\vert"],
+                q1 = ["\\|", "\\lVert", "\\rVert", "\\Vert"],
+                uo = function(n, t, o, s, u, p) {
                     let b, v, S, E, z = "",
                         F = 0;
                     b = S = E = n, v = null;
                     let N = "Size1-Regular";
-                    n === "\\uparrow" ? S = E = "\u23D0" : n === "\\Uparrow" ? S = E = "\u2016" : n === "\\downarrow" ? b = S = "\u23D0" : n === "\\Downarrow" ? b = S = "\u2016" : n === "\\updownarrow" ? (b = "\\uparrow", S = "\u23D0", E = "\\downarrow") : n === "\\Updownarrow" ? (b = "\\Uparrow", S = "\u2016", E = "\\Downarrow") : R.contains(T1, n) ? (S = "\u2223", z = "vert", F = 333) : R.contains(A1, n) ? (S = "\u2225", z = "doublevert", F = 556) : n === "[" || n === "\\lbrack" ? (b = "\u23A1", S = "\u23A2", E = "\u23A3", N = "Size4-Regular", z = "lbrack", F = 667) : n === "]" || n === "\\rbrack" ? (b = "\u23A4", S = "\u23A5", E = "\u23A6", N = "Size4-Regular", z = "rbrack", F = 667) : n === "\\lfloor" || n === "\u230A" ? (S = b = "\u23A2", E = "\u23A3", N = "Size4-Regular", z = "lfloor", F = 667) : n === "\\lceil" || n === "\u2308" ? (b = "\u23A1", S = E = "\u23A2", N = "Size4-Regular", z = "lceil", F = 667) : n === "\\rfloor" || n === "\u230B" ? (S = b = "\u23A5", E = "\u23A6", N = "Size4-Regular", z = "rfloor", F = 667) : n === "\\rceil" || n === "\u2309" ? (b = "\u23A4", S = E = "\u23A5", N = "Size4-Regular", z = "rceil", F = 667) : n === "(" || n === "\\lparen" ? (b = "\u239B", S = "\u239C", E = "\u239D", N = "Size4-Regular", z = "lparen", F = 875) : n === ")" || n === "\\rparen" ? (b = "\u239E", S = "\u239F", E = "\u23A0", N = "Size4-Regular", z = "rparen", F = 875) : n === "\\{" || n === "\\lbrace" ? (b = "\u23A7", v = "\u23A8", E = "\u23A9", S = "\u23AA", N = "Size4-Regular") : n === "\\}" || n === "\\rbrace" ? (b = "\u23AB", v = "\u23AC", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : n === "\\lgroup" || n === "\u27EE" ? (b = "\u23A7", E = "\u23A9", S = "\u23AA", N = "Size4-Regular") : n === "\\rgroup" || n === "\u27EF" ? (b = "\u23AB", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : n === "\\lmoustache" || n === "\u23B0" ? (b = "\u23A7", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : (n === "\\rmoustache" || n === "\u23B1") && (b = "\u23AB", E = "\u23A9", S = "\u23AA", N = "Size4-Regular");
-                    let O = _r(b, N, u),
-                        K = O.height + O.depth,
+                    n === "\\uparrow" ? S = E = "\u23D0" : n === "\\Uparrow" ? S = E = "\u2016" : n === "\\downarrow" ? b = S = "\u23D0" : n === "\\Downarrow" ? b = S = "\u2016" : n === "\\updownarrow" ? (b = "\\uparrow", S = "\u23D0", E = "\\downarrow") : n === "\\Updownarrow" ? (b = "\\Uparrow", S = "\u2016", E = "\\Downarrow") : R.contains(A1, n) ? (S = "\u2223", z = "vert", F = 333) : R.contains(q1, n) ? (S = "\u2225", z = "doublevert", F = 556) : n === "[" || n === "\\lbrack" ? (b = "\u23A1", S = "\u23A2", E = "\u23A3", N = "Size4-Regular", z = "lbrack", F = 667) : n === "]" || n === "\\rbrack" ? (b = "\u23A4", S = "\u23A5", E = "\u23A6", N = "Size4-Regular", z = "rbrack", F = 667) : n === "\\lfloor" || n === "\u230A" ? (S = b = "\u23A2", E = "\u23A3", N = "Size4-Regular", z = "lfloor", F = 667) : n === "\\lceil" || n === "\u2308" ? (b = "\u23A1", S = E = "\u23A2", N = "Size4-Regular", z = "lceil", F = 667) : n === "\\rfloor" || n === "\u230B" ? (S = b = "\u23A5", E = "\u23A6", N = "Size4-Regular", z = "rfloor", F = 667) : n === "\\rceil" || n === "\u2309" ? (b = "\u23A4", S = E = "\u23A5", N = "Size4-Regular", z = "rceil", F = 667) : n === "(" || n === "\\lparen" ? (b = "\u239B", S = "\u239C", E = "\u239D", N = "Size4-Regular", z = "lparen", F = 875) : n === ")" || n === "\\rparen" ? (b = "\u239E", S = "\u239F", E = "\u23A0", N = "Size4-Regular", z = "rparen", F = 875) : n === "\\{" || n === "\\lbrace" ? (b = "\u23A7", v = "\u23A8", E = "\u23A9", S = "\u23AA", N = "Size4-Regular") : n === "\\}" || n === "\\rbrace" ? (b = "\u23AB", v = "\u23AC", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : n === "\\lgroup" || n === "\u27EE" ? (b = "\u23A7", E = "\u23A9", S = "\u23AA", N = "Size4-Regular") : n === "\\rgroup" || n === "\u27EF" ? (b = "\u23AB", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : n === "\\lmoustache" || n === "\u23B0" ? (b = "\u23A7", E = "\u23AD", S = "\u23AA", N = "Size4-Regular") : (n === "\\rmoustache" || n === "\u23B1") && (b = "\u23AB", E = "\u23A9", S = "\u23AA", N = "Size4-Regular");
+                    let H = _r(b, N, u),
+                        K = H.height + H.depth,
                         ie = _r(S, N, u),
                         ye = ie.height + ie.depth,
                         ge = _r(E, N, u),
                         xe = ge.height + ge.depth,
                         ke = 0,
                         ze = 1;
                     if (v !== null) {
                         let Ve = _r(v, N, u);
                         ke = Ve.height + Ve.depth, ze = 2
                     }
                     let tt = K + xe + ke,
-                        Ze = Math.max(0, Math.ceil((t - tt) / (ze * ye))),
-                        pt = tt + Ze * ze * ye,
-                        lr = s.fontMetrics().axisHeight;
-                    o && (lr *= s.sizeMultiplier);
-                    let we = pt / 2 - lr,
+                        Qe = Math.max(0, Math.ceil((t - tt) / (ze * ye))),
+                        pt = tt + Qe * ze * ye,
+                        cr = s.fontMetrics().axisHeight;
+                    o && (cr *= s.sizeMultiplier);
+                    let we = pt / 2 - cr,
                         qe = [];
                     if (z.length > 0) {
                         let Ve = pt - K - xe,
                             $e = Math.round(pt * 1e3),
-                            ft = Bu(z, Math.round(Ve * 1e3)),
-                            K1 = new Ot(z, ft),
-                            Xo = (F / 1e3).toFixed(3) + "em",
-                            Jo = ($e / 1e3).toFixed(3) + "em",
-                            eh = new Et([K1], {
-                                width: Xo,
-                                height: Jo,
+                            ft = Nu(z, Math.round(Ve * 1e3)),
+                            eh = new Ot(z, ft),
+                            ta = (F / 1e3).toFixed(3) + "em",
+                            ra = ($e / 1e3).toFixed(3) + "em",
+                            th = new Et([eh], {
+                                width: ta,
+                                height: ra,
                                 viewBox: "0 0 " + F + " " + $e
                             }),
-                            a0 = B.makeSvgSpan([], [eh], s);
-                        a0.height = $e / 1e3, a0.style.width = Xo, a0.style.height = Jo, qe.push({
+                            s0 = B.makeSvgSpan([], [th], s);
+                        s0.height = $e / 1e3, s0.style.width = ta, s0.style.height = ra, qe.push({
                             type: "elem",
-                            elem: a0
+                            elem: s0
                         })
                     } else {
-                        if (qe.push(sn(E, N, u)), qe.push(t0), v === null) {
-                            let Ve = pt - K - xe + 2 * cn;
-                            qe.push(ln(S, Ve, s))
+                        if (qe.push(ln(E, N, u)), qe.push(r0), v === null) {
+                            let Ve = pt - K - xe + 2 * un;
+                            qe.push(cn(S, Ve, s))
                         } else {
-                            let Ve = (pt - K - xe - ke) / 2 + 2 * cn;
-                            qe.push(ln(S, Ve, s)), qe.push(t0), qe.push(sn(v, N, u)), qe.push(t0), qe.push(ln(S, Ve, s))
+                            let Ve = (pt - K - xe - ke) / 2 + 2 * un;
+                            qe.push(cn(S, Ve, s)), qe.push(r0), qe.push(ln(v, N, u)), qe.push(r0), qe.push(cn(S, Ve, s))
                         }
-                        qe.push(t0), qe.push(sn(b, N, u))
+                        qe.push(r0), qe.push(ln(b, N, u))
                     }
-                    let Fe = s.havingBaseStyle($.TEXT),
+                    let Fe = s.havingBaseStyle(G.TEXT),
                         Ne = B.makeVList({
                             positionType: "bottom",
                             positionData: we,
                             children: qe
                         }, Fe);
-                    return an(B.makeSpan(["delimsizing", "mult"], [Ne], Fe), $.TEXT, s, f)
+                    return sn(B.makeSpan(["delimsizing", "mult"], [Ne], Fe), G.TEXT, s, p)
                 },
-                un = 80,
-                hn = .08,
-                dn = function(n, t, o, s, u) {
-                    let f = Ru(n, s, o),
-                        b = new Ot(n, f),
+                hn = 80,
+                dn = .08,
+                mn = function(n, t, o, s, u) {
+                    let p = Fu(n, s, o),
+                        b = new Ot(n, p),
                         v = new Et([b], {
                             width: "400em",
-                            height: Q(t),
+                            height: Z(t),
                             viewBox: "0 0 400000 " + o,
                             preserveAspectRatio: "xMinYMin slice"
                         });
                     return B.makeSvgSpan(["hide-tail"], [v], u)
                 },
-                q1 = function(n, t) {
+                M1 = function(n, t) {
                     let o = t.havingBaseSizing(),
-                        s = uo("\\surd", n * o.sizeMultiplier, co, o),
+                        s = fo("\\surd", n * o.sizeMultiplier, po, o),
                         u = o.sizeMultiplier,
-                        f = Math.max(0, t.minRuleThickness - t.fontMetrics().sqrtRuleThickness),
+                        p = Math.max(0, t.minRuleThickness - t.fontMetrics().sqrtRuleThickness),
                         b, v = 0,
                         S = 0,
                         E = 0,
                         z;
-                    return s.type === "small" ? (E = 1e3 + 1e3 * f + un, n < 1 ? u = 1 : n < 1.4 && (u = .7), v = (1 + f + hn) / u, S = (1 + f) / u, b = dn("sqrtMain", v, E, f, t), b.style.minWidth = "0.853em", z = .833 / u) : s.type === "large" ? (E = (1e3 + un) * Sr[s.size], S = (Sr[s.size] + f) / u, v = (Sr[s.size] + f + hn) / u, b = dn("sqrtSize" + s.size, v, E, f, t), b.style.minWidth = "1.02em", z = 1 / u) : (v = n + f + hn, S = n + f, E = Math.floor(1e3 * n + f) + un, b = dn("sqrtTall", v, E, f, t), b.style.minWidth = "0.742em", z = 1.056), b.height = S, b.style.height = Q(v), {
+                    return s.type === "small" ? (E = 1e3 + 1e3 * p + hn, n < 1 ? u = 1 : n < 1.4 && (u = .7), v = (1 + p + dn) / u, S = (1 + p) / u, b = mn("sqrtMain", v, E, p, t), b.style.minWidth = "0.853em", z = .833 / u) : s.type === "large" ? (E = (1e3 + hn) * Sr[s.size], S = (Sr[s.size] + p) / u, v = (Sr[s.size] + p + dn) / u, b = mn("sqrtSize" + s.size, v, E, p, t), b.style.minWidth = "1.02em", z = 1 / u) : (v = n + p + dn, S = n + p, E = Math.floor(1e3 * n + p) + hn, b = mn("sqrtTall", v, E, p, t), b.style.minWidth = "0.742em", z = 1.056), b.height = S, b.style.height = Z(v), {
                         span: b,
                         advanceWidth: z,
-                        ruleWidth: (t.fontMetrics().sqrtRuleThickness + f) * u
+                        ruleWidth: (t.fontMetrics().sqrtRuleThickness + p) * u
                     }
                 },
-                so = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "\u230A", "\u230B", "\\lceil", "\\rceil", "\u2308", "\u2309", "\\surd"],
-                M1 = ["\\uparrow", "\\downarrow", "\\updownarrow", "\\Uparrow", "\\Downarrow", "\\Updownarrow", "|", "\\|", "\\vert", "\\Vert", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "\u27EE", "\u27EF", "\\lmoustache", "\\rmoustache", "\u23B0", "\u23B1"],
-                lo = ["<", ">", "\\langle", "\\rangle", "/", "\\backslash", "\\lt", "\\gt"],
+                ho = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "\u230A", "\u230B", "\\lceil", "\\rceil", "\u2308", "\u2309", "\\surd"],
+                E1 = ["\\uparrow", "\\downarrow", "\\updownarrow", "\\Uparrow", "\\Downarrow", "\\Updownarrow", "|", "\\|", "\\vert", "\\Vert", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "\u27EE", "\u27EF", "\\lmoustache", "\\rmoustache", "\u23B0", "\u23B1"],
+                mo = ["<", ">", "\\langle", "\\rangle", "/", "\\backslash", "\\lt", "\\gt"],
                 Sr = [0, 1.2, 1.8, 2.4, 3],
-                E1 = function(n, t, o, s, u) {
-                    if (n === "<" || n === "\\lt" || n === "\u27E8" ? n = "\\langle" : (n === ">" || n === "\\gt" || n === "\u27E9") && (n = "\\rangle"), R.contains(so, n) || R.contains(lo, n)) return oo(n, t, !1, o, s, u);
-                    if (R.contains(M1, n)) return ao(n, Sr[t], !1, o, s, u);
+                D1 = function(n, t, o, s, u) {
+                    if (n === "<" || n === "\\lt" || n === "\u27E8" ? n = "\\langle" : (n === ">" || n === "\\gt" || n === "\u27E9") && (n = "\\rangle"), R.contains(ho, n) || R.contains(mo, n)) return co(n, t, !1, o, s, u);
+                    if (R.contains(E1, n)) return uo(n, Sr[t], !1, o, s, u);
                     throw new a("Illegal delimiter: '" + n + "'")
                 },
-                D1 = [{
+                z1 = [{
                     type: "small",
-                    style: $.SCRIPTSCRIPT
+                    style: G.SCRIPTSCRIPT
                 }, {
                     type: "small",
-                    style: $.SCRIPT
+                    style: G.SCRIPT
                 }, {
                     type: "small",
-                    style: $.TEXT
+                    style: G.TEXT
                 }, {
                     type: "large",
                     size: 1
                 }, {
                     type: "large",
                     size: 2
                 }, {
                     type: "large",
                     size: 3
                 }, {
                     type: "large",
                     size: 4
                 }],
-                z1 = [{
+                R1 = [{
                     type: "small",
-                    style: $.SCRIPTSCRIPT
+                    style: G.SCRIPTSCRIPT
                 }, {
                     type: "small",
-                    style: $.SCRIPT
+                    style: G.SCRIPT
                 }, {
                     type: "small",
-                    style: $.TEXT
+                    style: G.TEXT
                 }, {
                     type: "stack"
                 }],
-                co = [{
+                po = [{
                     type: "small",
-                    style: $.SCRIPTSCRIPT
+                    style: G.SCRIPTSCRIPT
                 }, {
                     type: "small",
-                    style: $.SCRIPT
+                    style: G.SCRIPT
                 }, {
                     type: "small",
-                    style: $.TEXT
+                    style: G.TEXT
                 }, {
                     type: "large",
                     size: 1
                 }, {
                     type: "large",
                     size: 2
                 }, {
@@ -11145,55 +11145,55 @@
                     size: 3
                 }, {
                     type: "large",
                     size: 4
                 }, {
                     type: "stack"
                 }],
-                R1 = function(n) {
+                F1 = function(n) {
                     if (n.type === "small") return "Main-Regular";
                     if (n.type === "large") return "Size" + n.size + "-Regular";
                     if (n.type === "stack") return "Size4-Regular";
                     throw new Error("Add support for delim type '" + n.type + "' here.")
                 },
-                uo = function(n, t, o, s) {
+                fo = function(n, t, o, s) {
                     let u = Math.min(2, 3 - s.style.size);
-                    for (let f = u; f < o.length && o[f].type !== "stack"; f++) {
-                        let b = _r(n, R1(o[f]), "math"),
+                    for (let p = u; p < o.length && o[p].type !== "stack"; p++) {
+                        let b = _r(n, F1(o[p]), "math"),
                             v = b.height + b.depth;
-                        if (o[f].type === "small") {
-                            let S = s.havingBaseStyle(o[f].style);
+                        if (o[p].type === "small") {
+                            let S = s.havingBaseStyle(o[p].style);
                             v *= S.sizeMultiplier
                         }
-                        if (v > t) return o[f]
+                        if (v > t) return o[p]
                     }
                     return o[o.length - 1]
                 },
-                ho = function(n, t, o, s, u, f) {
+                go = function(n, t, o, s, u, p) {
                     n === "<" || n === "\\lt" || n === "\u27E8" ? n = "\\langle" : (n === ">" || n === "\\gt" || n === "\u27E9") && (n = "\\rangle");
                     let b;
-                    R.contains(lo, n) ? b = D1 : R.contains(so, n) ? b = co : b = z1;
-                    let v = uo(n, t, b, s);
-                    return v.type === "small" ? S1(n, v.style, o, s, u, f) : v.type === "large" ? oo(n, v.size, o, s, u, f) : ao(n, t, o, s, u, f)
+                    R.contains(mo, n) ? b = z1 : R.contains(ho, n) ? b = po : b = R1;
+                    let v = fo(n, t, b, s);
+                    return v.type === "small" ? C1(n, v.style, o, s, u, p) : v.type === "large" ? co(n, v.size, o, s, u, p) : uo(n, t, o, s, u, p)
                 };
             var Bt = {
-                sqrtImage: q1,
-                sizedDelim: E1,
+                sqrtImage: M1,
+                sizedDelim: D1,
                 sizeToMaxHeight: Sr,
-                customSizedDelim: ho,
-                leftRightDelim: function(n, t, o, s, u, f) {
+                customSizedDelim: go,
+                leftRightDelim: function(n, t, o, s, u, p) {
                     let b = s.fontMetrics().axisHeight * s.sizeMultiplier,
                         v = 901,
                         S = 5 / s.fontMetrics().ptPerEm,
                         E = Math.max(t - b, o + b),
                         z = Math.max(E / 500 * v, 2 * E - S);
-                    return ho(n, z, !0, s, u, f)
+                    return go(n, z, !0, s, u, p)
                 }
             };
-            let mo = {
+            let bo = {
                     "\\bigl": {
                         mclass: "mopen",
                         size: 1
                     },
                     "\\Bigl": {
                         mclass: "mopen",
                         size: 2
@@ -11251,136 +11251,136 @@
                         size: 3
                     },
                     "\\Bigg": {
                         mclass: "mord",
                         size: 4
                     }
                 },
-                F1 = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "\u230A", "\u230B", "\\lceil", "\\rceil", "\u2308", "\u2309", "<", ">", "\\langle", "\u27E8", "\\rangle", "\u27E9", "\\lt", "\\gt", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "\u27EE", "\u27EF", "\\lmoustache", "\\rmoustache", "\u23B0", "\u23B1", "/", "\\backslash", "|", "\\vert", "\\|", "\\Vert", "\\uparrow", "\\Uparrow", "\\downarrow", "\\Downarrow", "\\updownarrow", "\\Updownarrow", "."];
+                B1 = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "\u230A", "\u230B", "\\lceil", "\\rceil", "\u2308", "\u2309", "<", ">", "\\langle", "\u27E8", "\\rangle", "\u27E9", "\\lt", "\\gt", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "\u27EE", "\u27EF", "\\lmoustache", "\\rmoustache", "\u23B0", "\u23B1", "/", "\\backslash", "|", "\\vert", "\\|", "\\Vert", "\\uparrow", "\\Uparrow", "\\downarrow", "\\Downarrow", "\\updownarrow", "\\Updownarrow", "."];
 
-            function r0(n, t) {
-                let o = Jr(n);
-                if (o && R.contains(F1, o.text)) return o;
+            function n0(n, t) {
+                let o = Kr(n);
+                if (o && R.contains(B1, o.text)) return o;
                 throw o ? new a("Invalid delimiter '" + o.text + "' after '" + t.funcName + "'", n) : new a("Invalid delimiter type '" + n.type + "'", n)
             }
-            Z({
+            Q({
                 type: "delimsizing",
                 names: ["\\bigl", "\\Bigl", "\\biggl", "\\Biggl", "\\bigr", "\\Bigr", "\\biggr", "\\Biggr", "\\bigm", "\\Bigm", "\\biggm", "\\Biggm", "\\big", "\\Big", "\\bigg", "\\Bigg"],
                 props: {
                     numArgs: 1,
                     argTypes: ["primitive"]
                 },
                 handler: (n, t) => {
-                    let o = r0(t[0], n);
+                    let o = n0(t[0], n);
                     return {
                         type: "delimsizing",
                         mode: n.parser.mode,
-                        size: mo[n.funcName].size,
-                        mclass: mo[n.funcName].mclass,
+                        size: bo[n.funcName].size,
+                        mclass: bo[n.funcName].mclass,
                         delim: o.text
                     }
                 },
                 htmlBuilder: (n, t) => n.delim === "." ? B.makeSpan([n.mclass]) : Bt.sizedDelim(n.delim, n.size, t, n.mode, [n.mclass]),
                 mathmlBuilder: n => {
                     let t = [];
                     n.delim !== "." && t.push(dt(n.delim, n.mode));
                     let o = new V.MathNode("mo", t);
                     n.mclass === "mopen" || n.mclass === "mclose" ? o.setAttribute("fence", "true") : o.setAttribute("fence", "false"), o.setAttribute("stretchy", "true");
-                    let s = Q(Bt.sizeToMaxHeight[n.size]);
+                    let s = Z(Bt.sizeToMaxHeight[n.size]);
                     return o.setAttribute("minsize", s), o.setAttribute("maxsize", s), o
                 }
             });
 
-            function po(n) {
+            function yo(n) {
                 if (!n.body) throw new Error("Bug: The leftright ParseNode wasn't fully parsed.")
             }
-            Z({
+            Q({
                 type: "leftright-right",
                 names: ["\\right"],
                 props: {
                     numArgs: 1,
                     primitive: !0
                 },
                 handler: (n, t) => {
                     let o = n.parser.gullet.macros.get("\\current@color");
                     if (o && typeof o != "string") throw new a("\\current@color set to non-string in \\right");
                     return {
                         type: "leftright-right",
                         mode: n.parser.mode,
-                        delim: r0(t[0], n).text,
+                        delim: n0(t[0], n).text,
                         color: o
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "leftright",
                 names: ["\\left"],
                 props: {
                     numArgs: 1,
                     primitive: !0
                 },
                 handler: (n, t) => {
-                    let o = r0(t[0], n),
+                    let o = n0(t[0], n),
                         s = n.parser;
                     ++s.leftrightDepth;
                     let u = s.parseExpression(!1);
                     --s.leftrightDepth, s.expect("\\right", !1);
-                    let f = de(s.parseFunction(), "leftright-right");
+                    let p = de(s.parseFunction(), "leftright-right");
                     return {
                         type: "leftright",
                         mode: s.mode,
                         body: u,
                         left: o.text,
-                        right: f.delim,
-                        rightColor: f.color
+                        right: p.delim,
+                        rightColor: p.color
                     }
                 },
                 htmlBuilder: (n, t) => {
-                    po(n);
-                    let o = Qe(n.body, t, !0, ["mopen", "mclose"]),
+                    yo(n);
+                    let o = Ze(n.body, t, !0, ["mopen", "mclose"]),
                         s = 0,
                         u = 0,
-                        f = !1;
-                    for (let S = 0; S < o.length; S++) o[S].isMiddle ? f = !0 : (s = Math.max(o[S].height, s), u = Math.max(o[S].depth, u));
+                        p = !1;
+                    for (let S = 0; S < o.length; S++) o[S].isMiddle ? p = !0 : (s = Math.max(o[S].height, s), u = Math.max(o[S].depth, u));
                     s *= t.sizeMultiplier, u *= t.sizeMultiplier;
                     let b;
-                    if (n.left === "." ? b = wr(t, ["mopen"]) : b = Bt.leftRightDelim(n.left, s, u, t, n.mode, ["mopen"]), o.unshift(b), f)
+                    if (n.left === "." ? b = wr(t, ["mopen"]) : b = Bt.leftRightDelim(n.left, s, u, t, n.mode, ["mopen"]), o.unshift(b), p)
                         for (let S = 1; S < o.length; S++) {
                             let z = o[S].isMiddle;
                             z && (o[S] = Bt.leftRightDelim(z.delim, s, u, z.options, n.mode, []))
                         }
                     let v;
                     if (n.right === ".") v = wr(t, ["mclose"]);
                     else {
                         let S = n.rightColor ? t.withColor(n.rightColor) : t;
                         v = Bt.leftRightDelim(n.right, s, u, S, n.mode, ["mclose"])
                     }
                     return o.push(v), B.makeSpan(["minner"], o, t)
                 },
                 mathmlBuilder: (n, t) => {
-                    po(n);
+                    yo(n);
                     let o = it(n.body, t);
                     if (n.left !== ".") {
                         let s = new V.MathNode("mo", [dt(n.left, n.mode)]);
                         s.setAttribute("fence", "true"), o.unshift(s)
                     }
                     if (n.right !== ".") {
                         let s = new V.MathNode("mo", [dt(n.right, n.mode)]);
                         s.setAttribute("fence", "true"), n.rightColor && s.setAttribute("mathcolor", n.rightColor), o.push(s)
                     }
-                    return en(o)
+                    return tn(o)
                 }
-            }), Z({
+            }), Q({
                 type: "middle",
                 names: ["\\middle"],
                 props: {
                     numArgs: 1,
                     primitive: !0
                 },
                 handler: (n, t) => {
-                    let o = r0(t[0], n);
+                    let o = n0(t[0], n);
                     if (!n.parser.leftrightDepth) throw new a("\\middle without preceding \\left", o);
                     return {
                         type: "middle",
                         mode: n.parser.mode,
                         delim: o.text
                     }
                 },
@@ -11399,56 +11399,56 @@
                 },
                 mathmlBuilder: (n, t) => {
                     let o = n.delim === "\\vert" || n.delim === "|" ? dt("|", "text") : dt(n.delim, n.mode),
                         s = new V.MathNode("mo", [o]);
                     return s.setAttribute("fence", "true"), s.setAttribute("lspace", "0.05em"), s.setAttribute("rspace", "0.05em"), s
                 }
             });
-            let mn = (n, t) => {
+            let pn = (n, t) => {
                     let o = B.wrapFragment(ve(n.body, t), t),
                         s = n.label.slice(1),
                         u = t.sizeMultiplier,
-                        f, b = 0,
+                        p, b = 0,
                         v = R.isCharacterBox(n.body);
-                    if (s === "sout") f = B.makeSpan(["stretchy", "sout"]), f.height = t.fontMetrics().defaultRuleThickness / u, b = -.5 * t.fontMetrics().xHeight;
+                    if (s === "sout") p = B.makeSpan(["stretchy", "sout"]), p.height = t.fontMetrics().defaultRuleThickness / u, b = -.5 * t.fontMetrics().xHeight;
                     else if (s === "phase") {
                         let E = Ie({
                                 number: .6,
                                 unit: "pt"
                             }, t),
                             z = Ie({
                                 number: .35,
                                 unit: "ex"
                             }, t),
                             F = t.havingBaseSizing();
                         u = u / F.sizeMultiplier;
                         let N = o.height + o.depth + E + z;
-                        o.style.paddingLeft = Q(N / 2 + E);
-                        let O = Math.floor(1e3 * N * u),
-                            K = Du(O),
+                        o.style.paddingLeft = Z(N / 2 + E);
+                        let H = Math.floor(1e3 * N * u),
+                            K = zu(H),
                             ie = new Et([new Ot("phase", K)], {
                                 width: "400em",
-                                height: Q(O / 1e3),
-                                viewBox: "0 0 400000 " + O,
+                                height: Z(H / 1e3),
+                                viewBox: "0 0 400000 " + H,
                                 preserveAspectRatio: "xMinYMin slice"
                             });
-                        f = B.makeSvgSpan(["hide-tail"], [ie], t), f.style.height = Q(N), b = o.depth + E + z
+                        p = B.makeSvgSpan(["hide-tail"], [ie], t), p.style.height = Z(N), b = o.depth + E + z
                     } else {
                         /cancel/.test(s) ? v || o.classes.push("cancel-pad") : s === "angl" ? o.classes.push("anglpad") : o.classes.push("boxpad");
                         let E = 0,
                             z = 0,
                             F = 0;
-                        /box/.test(s) ? (F = Math.max(t.fontMetrics().fboxrule, t.minRuleThickness), E = t.fontMetrics().fboxsep + (s === "colorbox" ? 0 : F), z = E) : s === "angl" ? (F = Math.max(t.fontMetrics().defaultRuleThickness, t.minRuleThickness), E = 4 * F, z = Math.max(0, .25 - o.depth)) : (E = v ? .2 : 0, z = E), f = Ft.encloseSpan(o, s, E, z, t), /fbox|boxed|fcolorbox/.test(s) ? (f.style.borderStyle = "solid", f.style.borderWidth = Q(F)) : s === "angl" && F !== .049 && (f.style.borderTopWidth = Q(F), f.style.borderRightWidth = Q(F)), b = o.depth + z, n.backgroundColor && (f.style.backgroundColor = n.backgroundColor, n.borderColor && (f.style.borderColor = n.borderColor))
+                        /box/.test(s) ? (F = Math.max(t.fontMetrics().fboxrule, t.minRuleThickness), E = t.fontMetrics().fboxsep + (s === "colorbox" ? 0 : F), z = E) : s === "angl" ? (F = Math.max(t.fontMetrics().defaultRuleThickness, t.minRuleThickness), E = 4 * F, z = Math.max(0, .25 - o.depth)) : (E = v ? .2 : 0, z = E), p = Ft.encloseSpan(o, s, E, z, t), /fbox|boxed|fcolorbox/.test(s) ? (p.style.borderStyle = "solid", p.style.borderWidth = Z(F)) : s === "angl" && F !== .049 && (p.style.borderTopWidth = Z(F), p.style.borderRightWidth = Z(F)), b = o.depth + z, n.backgroundColor && (p.style.backgroundColor = n.backgroundColor, n.borderColor && (p.style.borderColor = n.borderColor))
                     }
                     let S;
                     if (n.backgroundColor) S = B.makeVList({
                         positionType: "individualShift",
                         children: [{
                             type: "elem",
-                            elem: f,
+                            elem: p,
                             shift: b
                         }, {
                             type: "elem",
                             elem: o,
                             shift: 0
                         }]
                     }, t);
@@ -11458,23 +11458,23 @@
                             positionType: "individualShift",
                             children: [{
                                 type: "elem",
                                 elem: o,
                                 shift: 0
                             }, {
                                 type: "elem",
-                                elem: f,
+                                elem: p,
                                 shift: b,
                                 wrapperClasses: E
                             }]
                         }, t)
                     }
                     return /cancel/.test(s) && (S.height = o.height, S.depth = o.depth), /cancel/.test(s) && !v ? B.makeSpan(["mord", "cancel-lap"], [S], t) : B.makeSpan(["mord"], [S], t)
                 },
-                pn = (n, t) => {
+                fn = (n, t) => {
                     let o = 0,
                         s = new V.MathNode(n.label.indexOf("colorbox") > -1 ? "mpadded" : "menclose", [Ee(n.body, t)]);
                     switch (n.label) {
                         case "\\cancel":
                             s.setAttribute("notation", "updiagonalstrike");
                             break;
                         case "\\bcancel":
@@ -11501,62 +11501,62 @@
                             break;
                         case "\\xcancel":
                             s.setAttribute("notation", "updiagonalstrike downdiagonalstrike");
                             break
                     }
                     return n.backgroundColor && s.setAttribute("mathbackground", n.backgroundColor), s
                 };
-            Z({
+            Q({
                 type: "enclose",
                 names: ["\\colorbox"],
                 props: {
                     numArgs: 2,
                     allowedInText: !0,
                     argTypes: ["color", "text"]
                 },
                 handler(n, t, o) {
                     let {
                         parser: s,
                         funcName: u
-                    } = n, f = de(t[0], "color-token").color, b = t[1];
+                    } = n, p = de(t[0], "color-token").color, b = t[1];
                     return {
                         type: "enclose",
                         mode: s.mode,
                         label: u,
-                        backgroundColor: f,
+                        backgroundColor: p,
                         body: b
                     }
                 },
-                htmlBuilder: mn,
-                mathmlBuilder: pn
-            }), Z({
+                htmlBuilder: pn,
+                mathmlBuilder: fn
+            }), Q({
                 type: "enclose",
                 names: ["\\fcolorbox"],
                 props: {
                     numArgs: 3,
                     allowedInText: !0,
                     argTypes: ["color", "color", "text"]
                 },
                 handler(n, t, o) {
                     let {
                         parser: s,
                         funcName: u
-                    } = n, f = de(t[0], "color-token").color, b = de(t[1], "color-token").color, v = t[2];
+                    } = n, p = de(t[0], "color-token").color, b = de(t[1], "color-token").color, v = t[2];
                     return {
                         type: "enclose",
                         mode: s.mode,
                         label: u,
                         backgroundColor: b,
-                        borderColor: f,
+                        borderColor: p,
                         body: v
                     }
                 },
-                htmlBuilder: mn,
-                mathmlBuilder: pn
-            }), Z({
+                htmlBuilder: pn,
+                mathmlBuilder: fn
+            }), Q({
                 type: "enclose",
                 names: ["\\fbox"],
                 props: {
                     numArgs: 1,
                     argTypes: ["hbox"],
                     allowedInText: !0
                 },
@@ -11567,15 +11567,15 @@
                     return {
                         type: "enclose",
                         mode: o.mode,
                         label: "\\fbox",
                         body: t[0]
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "enclose",
                 names: ["\\cancel", "\\bcancel", "\\xcancel", "\\sout", "\\phase"],
                 props: {
                     numArgs: 1
                 },
                 handler(n, t) {
                     let {
@@ -11585,17 +11585,17 @@
                     return {
                         type: "enclose",
                         mode: o.mode,
                         label: s,
                         body: u
                     }
                 },
-                htmlBuilder: mn,
-                mathmlBuilder: pn
-            }), Z({
+                htmlBuilder: pn,
+                mathmlBuilder: fn
+            }), Q({
                 type: "enclose",
                 names: ["\\angl"],
                 props: {
                     numArgs: 1,
                     argTypes: ["hbox"],
                     allowedInText: !1
                 },
@@ -11607,38 +11607,38 @@
                         type: "enclose",
                         mode: o.mode,
                         label: "\\angl",
                         body: t[0]
                     }
                 }
             });
-            let fo = {};
+            let xo = {};
 
             function wt(n) {
                 let {
                     type: t,
                     names: o,
                     props: s,
                     handler: u,
-                    htmlBuilder: f,
+                    htmlBuilder: p,
                     mathmlBuilder: b
                 } = n, v = {
                     type: t,
                     numArgs: s.numArgs || 0,
                     allowedInText: !1,
                     numOptionalArgs: 0,
                     handler: u
                 };
-                for (let S = 0; S < o.length; ++S) fo[o[S]] = v;
-                f && (Yr[t] = f), b && (Qr[t] = b)
+                for (let S = 0; S < o.length; ++S) xo[o[S]] = v;
+                p && (Zr[t] = p), b && (Qr[t] = b)
             }
-            let go = {};
+            let vo = {};
 
-            function w(n, t) {
-                go[n] = t
+            function k(n, t) {
+                vo[n] = t
             }
             class st {
                 constructor(t, o, s) {
                     this.lexer = void 0, this.start = void 0, this.end = void 0, this.lexer = t, this.start = o, this.end = s
                 }
                 static range(t, o) {
                     return o ? !t || !t.loc || !o.loc || t.loc.lexer !== o.loc.lexer ? null : new st(t.loc.lexer, t.loc.start, o.loc.end) : t && t.loc
@@ -11649,180 +11649,180 @@
                     this.text = void 0, this.loc = void 0, this.noexpand = void 0, this.treatAsRelax = void 0, this.text = t, this.loc = o
                 }
                 range(t, o) {
                     return new mt(o, st.range(this, t))
                 }
             }
 
-            function bo(n) {
+            function wo(n) {
                 let t = [];
                 n.consumeSpaces();
                 let o = n.fetch().text;
                 for (o === "\\relax" && (n.consume(), n.consumeSpaces(), o = n.fetch().text); o === "\\hline" || o === "\\hdashline";) n.consume(), t.push(o === "\\hdashline"), n.consumeSpaces(), o = n.fetch().text;
                 return t
             }
-            let n0 = n => {
+            let i0 = n => {
                 if (!n.parser.settings.displayMode) throw new a("{" + n.envName + "} can be used only in display mode.")
             };
 
-            function fn(n) {
+            function gn(n) {
                 if (n.indexOf("ed") === -1) return n.indexOf("*") === -1
             }
 
             function $t(n, t, o) {
                 let {
                     hskipBeforeAndAfter: s,
                     addJot: u,
-                    cols: f,
+                    cols: p,
                     arraystretch: b,
                     colSeparationType: v,
                     autoTag: S,
                     singleRow: E,
                     emptySingleRow: z,
                     maxNumCols: F,
                     leqno: N
                 } = t;
                 if (n.gullet.beginGroup(), E || n.gullet.macros.set("\\cr", "\\\\\\relax"), !b) {
                     let ze = n.gullet.expandMacroAsText("\\arraystretch");
                     if (ze == null) b = 1;
                     else if (b = parseFloat(ze), !b || b < 0) throw new a("Invalid \\arraystretch: " + ze)
                 }
                 n.gullet.beginGroup();
-                let O = [],
-                    K = [O],
+                let H = [],
+                    K = [H],
                     ie = [],
                     ye = [],
                     ge = S != null ? [] : void 0;
 
                 function xe() {
                     S && n.gullet.macros.set("\\@eqnsw", "1", !0)
                 }
 
                 function ke() {
                     ge && (n.gullet.macros.get("\\df@tag") ? (ge.push(n.subparse([new mt("\\df@tag")])), n.gullet.macros.set("\\df@tag", void 0, !0)) : ge.push(!!S && n.gullet.macros.get("\\@eqnsw") === "1"))
                 }
-                for (xe(), ye.push(bo(n));;) {
+                for (xe(), ye.push(wo(n));;) {
                     let ze = n.parseExpression(!1, E ? "\\end" : "\\\\");
                     n.gullet.endGroup(), n.gullet.beginGroup(), ze = {
                         type: "ordgroup",
                         mode: n.mode,
                         body: ze
                     }, o && (ze = {
                         type: "styling",
                         mode: n.mode,
                         style: o,
                         body: [ze]
-                    }), O.push(ze);
+                    }), H.push(ze);
                     let tt = n.fetch().text;
                     if (tt === "&") {
-                        if (F && O.length === F) {
+                        if (F && H.length === F) {
                             if (E || v) throw new a("Too many tab characters: &", n.nextToken);
                             n.settings.reportNonstrict("textEnv", "Too few columns specified in the {array} column argument.")
                         }
                         n.consume()
                     } else if (tt === "\\end") {
-                        ke(), O.length === 1 && ze.type === "styling" && ze.body[0].body.length === 0 && (K.length > 1 || !z) && K.pop(), ye.length < K.length + 1 && ye.push([]);
+                        ke(), H.length === 1 && ze.type === "styling" && ze.body[0].body.length === 0 && (K.length > 1 || !z) && K.pop(), ye.length < K.length + 1 && ye.push([]);
                         break
                     } else if (tt === "\\\\") {
                         n.consume();
-                        let Ze;
-                        n.gullet.future().text !== " " && (Ze = n.parseSizeGroup(!0)), ie.push(Ze ? Ze.value : null), ke(), ye.push(bo(n)), O = [], K.push(O), xe()
+                        let Qe;
+                        n.gullet.future().text !== " " && (Qe = n.parseSizeGroup(!0)), ie.push(Qe ? Qe.value : null), ke(), ye.push(wo(n)), H = [], K.push(H), xe()
                     } else throw new a("Expected & or \\\\ or \\cr or \\end", n.nextToken)
                 }
                 return n.gullet.endGroup(), n.gullet.endGroup(), {
                     type: "array",
                     mode: n.mode,
                     addJot: u,
                     arraystretch: b,
                     body: K,
-                    cols: f,
+                    cols: p,
                     rowGaps: ie,
                     hskipBeforeAndAfter: s,
                     hLinesBeforeRow: ye,
                     colSeparationType: v,
                     tags: ge,
                     leqno: N
                 }
             }
 
-            function gn(n) {
+            function bn(n) {
                 return n.slice(0, 1) === "d" ? "display" : "text"
             }
             let kt = function(n, t) {
                     let o, s, u = n.body.length,
-                        f = n.hLinesBeforeRow,
+                        p = n.hLinesBeforeRow,
                         b = 0,
                         v = new Array(u),
                         S = [],
                         E = Math.max(t.fontMetrics().arrayRuleWidth, t.minRuleThickness),
                         z = 1 / t.fontMetrics().ptPerEm,
                         F = 5 * z;
-                    n.colSeparationType && n.colSeparationType === "small" && (F = .2778 * (t.havingStyle($.SCRIPT).sizeMultiplier / t.sizeMultiplier));
+                    n.colSeparationType && n.colSeparationType === "small" && (F = .2778 * (t.havingStyle(G.SCRIPT).sizeMultiplier / t.sizeMultiplier));
                     let N = n.colSeparationType === "CD" ? Ie({
                             number: 3,
                             unit: "ex"
                         }, t) : 12 * z,
-                        O = 3 * z,
+                        H = 3 * z,
                         K = n.arraystretch * N,
                         ie = .7 * K,
                         ye = .3 * K,
                         ge = 0;
 
                     function xe(we) {
                         for (let qe = 0; qe < we.length; ++qe) qe > 0 && (ge += .25), S.push({
                             pos: ge,
                             isDashed: we[qe]
                         })
                     }
-                    for (xe(f[0]), o = 0; o < n.body.length; ++o) {
+                    for (xe(p[0]), o = 0; o < n.body.length; ++o) {
                         let we = n.body[o],
                             qe = ie,
                             Fe = ye;
                         b < we.length && (b = we.length);
                         let Ne = new Array(we.length);
                         for (s = 0; s < we.length; ++s) {
                             let ft = ve(we[s], t);
                             Fe < ft.depth && (Fe = ft.depth), qe < ft.height && (qe = ft.height), Ne[s] = ft
                         }
                         let Ve = n.rowGaps[o],
                             $e = 0;
-                        Ve && ($e = Ie(Ve, t), $e > 0 && ($e += ye, Fe < $e && (Fe = $e), $e = 0)), n.addJot && (Fe += O), Ne.height = qe, Ne.depth = Fe, ge += qe, Ne.pos = ge, ge += Fe + $e, v[o] = Ne, xe(f[o + 1])
+                        Ve && ($e = Ie(Ve, t), $e > 0 && ($e += ye, Fe < $e && (Fe = $e), $e = 0)), n.addJot && (Fe += H), Ne.height = qe, Ne.depth = Fe, ge += qe, Ne.pos = ge, ge += Fe + $e, v[o] = Ne, xe(p[o + 1])
                     }
                     let ke = ge / 2 + t.fontMetrics().axisHeight,
                         ze = n.cols || [],
                         tt = [],
-                        Ze, pt, lr = [];
+                        Qe, pt, cr = [];
                     if (n.tags && n.tags.some(we => we))
                         for (o = 0; o < u; ++o) {
                             let we = v[o],
                                 qe = we.pos - ke,
                                 Fe = n.tags[o],
                                 Ne;
-                            Fe === !0 ? Ne = B.makeSpan(["eqn-num"], [], t) : Fe === !1 ? Ne = B.makeSpan([], [], t) : Ne = B.makeSpan([], Qe(Fe, t, !0), t), Ne.depth = we.depth, Ne.height = we.height, lr.push({
+                            Fe === !0 ? Ne = B.makeSpan(["eqn-num"], [], t) : Fe === !1 ? Ne = B.makeSpan([], [], t) : Ne = B.makeSpan([], Ze(Fe, t, !0), t), Ne.depth = we.depth, Ne.height = we.height, cr.push({
                                 type: "elem",
                                 elem: Ne,
                                 shift: qe
                             })
                         }
                     for (s = 0, pt = 0; s < b || pt < ze.length; ++s, ++pt) {
                         let we = ze[pt] || {},
                             qe = !0;
                         for (; we.type === "separator";) {
-                            if (qe || (Ze = B.makeSpan(["arraycolsep"], []), Ze.style.width = Q(t.fontMetrics().doubleRuleSep), tt.push(Ze)), we.separator === "|" || we.separator === ":") {
+                            if (qe || (Qe = B.makeSpan(["arraycolsep"], []), Qe.style.width = Z(t.fontMetrics().doubleRuleSep), tt.push(Qe)), we.separator === "|" || we.separator === ":") {
                                 let Ve = we.separator === "|" ? "solid" : "dashed",
                                     $e = B.makeSpan(["vertical-separator"], [], t);
-                                $e.style.height = Q(ge), $e.style.borderRightWidth = Q(E), $e.style.borderRightStyle = Ve, $e.style.margin = "0 " + Q(-E / 2);
+                                $e.style.height = Z(ge), $e.style.borderRightWidth = Z(E), $e.style.borderRightStyle = Ve, $e.style.margin = "0 " + Z(-E / 2);
                                 let ft = ge - ke;
-                                ft && ($e.style.verticalAlign = Q(-ft)), tt.push($e)
+                                ft && ($e.style.verticalAlign = Z(-ft)), tt.push($e)
                             } else throw new a("Invalid separator type: " + we.separator);
                             pt++, we = ze[pt] || {}, qe = !1
                         }
                         if (s >= b) continue;
                         let Fe;
-                        (s > 0 || n.hskipBeforeAndAfter) && (Fe = R.deflt(we.pregap, F), Fe !== 0 && (Ze = B.makeSpan(["arraycolsep"], []), Ze.style.width = Q(Fe), tt.push(Ze)));
+                        (s > 0 || n.hskipBeforeAndAfter) && (Fe = R.deflt(we.pregap, F), Fe !== 0 && (Qe = B.makeSpan(["arraycolsep"], []), Qe.style.width = Z(Fe), tt.push(Qe)));
                         let Ne = [];
                         for (o = 0; o < u; ++o) {
                             let Ve = v[o],
                                 $e = Ve[s];
                             if (!$e) continue;
                             let ft = Ve.pos - ke;
                             $e.depth = Ve.depth, $e.height = Ve.height, Ne.push({
@@ -11830,15 +11830,15 @@
                                 elem: $e,
                                 shift: ft
                             })
                         }
                         Ne = B.makeVList({
                             positionType: "individualShift",
                             children: Ne
-                        }, t), Ne = B.makeSpan(["col-align-" + (we.align || "c")], [Ne]), tt.push(Ne), (s < b - 1 || n.hskipBeforeAndAfter) && (Fe = R.deflt(we.postgap, F), Fe !== 0 && (Ze = B.makeSpan(["arraycolsep"], []), Ze.style.width = Q(Fe), tt.push(Ze)))
+                        }, t), Ne = B.makeSpan(["col-align-" + (we.align || "c")], [Ne]), tt.push(Ne), (s < b - 1 || n.hskipBeforeAndAfter) && (Fe = R.deflt(we.postgap, F), Fe !== 0 && (Qe = B.makeSpan(["arraycolsep"], []), Qe.style.width = Z(Fe), tt.push(Qe)))
                     }
                     if (v = B.makeSpan(["mtable"], tt), S.length > 0) {
                         let we = B.makeLineSpan("hline", t, E),
                             qe = B.makeLineSpan("hdashline", t, E),
                             Fe = [{
                                 type: "elem",
                                 elem: v,
@@ -11858,74 +11858,74 @@
                             })
                         }
                         v = B.makeVList({
                             positionType: "individualShift",
                             children: Fe
                         }, t)
                     }
-                    if (lr.length === 0) return B.makeSpan(["mord"], [v], t);
+                    if (cr.length === 0) return B.makeSpan(["mord"], [v], t);
                     {
                         let we = B.makeVList({
                             positionType: "individualShift",
-                            children: lr
+                            children: cr
                         }, t);
                         return we = B.makeSpan(["tag"], [we], t), B.makeFragment([v, we])
                     }
                 },
-                B1 = {
+                N1 = {
                     c: "center ",
                     l: "left ",
                     r: "right "
                 },
                 _t = function(n, t) {
                     let o = [],
                         s = new V.MathNode("mtd", [], ["mtr-glue"]),
                         u = new V.MathNode("mtd", [], ["mml-eqn-num"]);
                     for (let F = 0; F < n.body.length; F++) {
                         let N = n.body[F],
-                            O = [];
-                        for (let K = 0; K < N.length; K++) O.push(new V.MathNode("mtd", [Ee(N[K], t)]));
-                        n.tags && n.tags[F] && (O.unshift(s), O.push(s), n.leqno ? O.unshift(u) : O.push(u)), o.push(new V.MathNode("mtr", O))
+                            H = [];
+                        for (let K = 0; K < N.length; K++) H.push(new V.MathNode("mtd", [Ee(N[K], t)]));
+                        n.tags && n.tags[F] && (H.unshift(s), H.push(s), n.leqno ? H.unshift(u) : H.push(u)), o.push(new V.MathNode("mtr", H))
                     }
-                    let f = new V.MathNode("mtable", o),
+                    let p = new V.MathNode("mtable", o),
                         b = n.arraystretch === .5 ? .1 : .16 + n.arraystretch - 1 + (n.addJot ? .09 : 0);
-                    f.setAttribute("rowspacing", Q(b));
+                    p.setAttribute("rowspacing", Z(b));
                     let v = "",
                         S = "";
                     if (n.cols && n.cols.length > 0) {
                         let F = n.cols,
                             N = "",
-                            O = !1,
+                            H = !1,
                             K = 0,
                             ie = F.length;
                         F[0].type === "separator" && (v += "top ", K = 1), F[F.length - 1].type === "separator" && (v += "bottom ", ie -= 1);
-                        for (let ye = K; ye < ie; ye++) F[ye].type === "align" ? (S += B1[F[ye].align], O && (N += "none "), O = !0) : F[ye].type === "separator" && O && (N += F[ye].separator === "|" ? "solid " : "dashed ", O = !1);
-                        f.setAttribute("columnalign", S.trim()), /[sd]/.test(N) && f.setAttribute("columnlines", N.trim())
+                        for (let ye = K; ye < ie; ye++) F[ye].type === "align" ? (S += N1[F[ye].align], H && (N += "none "), H = !0) : F[ye].type === "separator" && H && (N += F[ye].separator === "|" ? "solid " : "dashed ", H = !1);
+                        p.setAttribute("columnalign", S.trim()), /[sd]/.test(N) && p.setAttribute("columnlines", N.trim())
                     }
                     if (n.colSeparationType === "align") {
                         let F = n.cols || [],
                             N = "";
-                        for (let O = 1; O < F.length; O++) N += O % 2 ? "0em " : "1em ";
-                        f.setAttribute("columnspacing", N.trim())
-                    } else n.colSeparationType === "alignat" || n.colSeparationType === "gather" ? f.setAttribute("columnspacing", "0em") : n.colSeparationType === "small" ? f.setAttribute("columnspacing", "0.2778em") : n.colSeparationType === "CD" ? f.setAttribute("columnspacing", "0.5em") : f.setAttribute("columnspacing", "1em");
+                        for (let H = 1; H < F.length; H++) N += H % 2 ? "0em " : "1em ";
+                        p.setAttribute("columnspacing", N.trim())
+                    } else n.colSeparationType === "alignat" || n.colSeparationType === "gather" ? p.setAttribute("columnspacing", "0em") : n.colSeparationType === "small" ? p.setAttribute("columnspacing", "0.2778em") : n.colSeparationType === "CD" ? p.setAttribute("columnspacing", "0.5em") : p.setAttribute("columnspacing", "1em");
                     let E = "",
                         z = n.hLinesBeforeRow;
                     v += z[0].length > 0 ? "left " : "", v += z[z.length - 1].length > 0 ? "right " : "";
                     for (let F = 1; F < z.length - 1; F++) E += z[F].length === 0 ? "none " : z[F][0] ? "dashed " : "solid ";
-                    return /[sd]/.test(E) && f.setAttribute("rowlines", E.trim()), v !== "" && (f = new V.MathNode("menclose", [f]), f.setAttribute("notation", v.trim())), n.arraystretch && n.arraystretch < 1 && (f = new V.MathNode("mstyle", [f]), f.setAttribute("scriptlevel", "1")), f
+                    return /[sd]/.test(E) && p.setAttribute("rowlines", E.trim()), v !== "" && (p = new V.MathNode("menclose", [p]), p.setAttribute("notation", v.trim())), n.arraystretch && n.arraystretch < 1 && (p = new V.MathNode("mstyle", [p]), p.setAttribute("scriptlevel", "1")), p
                 },
-                yo = function(n, t) {
-                    n.envName.indexOf("ed") === -1 && n0(n);
+                ko = function(n, t) {
+                    n.envName.indexOf("ed") === -1 && i0(n);
                     let o = [],
                         s = n.envName.indexOf("at") > -1 ? "alignat" : "align",
                         u = n.envName === "split",
-                        f = $t(n.parser, {
+                        p = $t(n.parser, {
                             cols: o,
                             addJot: !0,
-                            autoTag: u ? void 0 : fn(n.envName),
+                            autoTag: u ? void 0 : gn(n.envName),
                             emptySingleRow: !0,
                             colSeparationType: s,
                             maxNumCols: u ? 2 : void 0,
                             leqno: n.parser.settings.leqno
                         }, "display"),
                         b, v = 0,
                         S = {
@@ -11938,15 +11938,15 @@
                         for (let F = 0; F < t[0].body.length; F++) {
                             let N = de(t[0].body[F], "textord");
                             z += N.text
                         }
                         b = Number(z), v = b * 2
                     }
                     let E = !v;
-                    f.body.forEach(function(z) {
+                    p.body.forEach(function(z) {
                         for (let F = 1; F < z.length; F += 2) {
                             let N = de(z[F], "styling");
                             de(N.body[0], "ordgroup").body.unshift(S)
                         }
                         if (E) v < z.length && (v = z.length);
                         else {
                             let F = z.length / 2;
@@ -11959,45 +11959,45 @@
                         z % 2 === 1 ? F = "l" : z > 0 && E && (N = 1), o[z] = {
                             type: "align",
                             align: F,
                             pregap: N,
                             postgap: 0
                         }
                     }
-                    return f.colSeparationType = E ? "align" : "alignat", f
+                    return p.colSeparationType = E ? "align" : "alignat", p
                 };
             wt({
                 type: "array",
                 names: ["array", "darray"],
                 props: {
                     numArgs: 1
                 },
                 handler(n, t) {
-                    let u = (Jr(t[0]) ? [t[0]] : de(t[0], "ordgroup").body).map(function(b) {
-                            let S = rn(b).text;
+                    let u = (Kr(t[0]) ? [t[0]] : de(t[0], "ordgroup").body).map(function(b) {
+                            let S = nn(b).text;
                             if ("lcr".indexOf(S) !== -1) return {
                                 type: "align",
                                 align: S
                             };
                             if (S === "|") return {
                                 type: "separator",
                                 separator: "|"
                             };
                             if (S === ":") return {
                                 type: "separator",
                                 separator: ":"
                             };
                             throw new a("Unknown column alignment: " + S, b)
                         }),
-                        f = {
+                        p = {
                             cols: u,
                             hskipBeforeAndAfter: !0,
                             maxNumCols: u.length
                         };
-                    return $t(n.parser, f, gn(n.envName))
+                    return $t(n.parser, p, bn(n.envName))
                 },
                 htmlBuilder: kt,
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["matrix", "pmatrix", "bmatrix", "Bmatrix", "vmatrix", "Vmatrix", "matrix*", "pmatrix*", "bmatrix*", "Bmatrix*", "vmatrix*", "Vmatrix*"],
                 props: {
@@ -12026,17 +12026,17 @@
                             if (b.consume(), b.consumeSpaces(), o = b.fetch().text, "lcr".indexOf(o) === -1) throw new a("Expected l or c or r", b.nextToken);
                             b.consume(), b.consumeSpaces(), b.expect("]"), b.consume(), s.cols = [{
                                 type: "align",
                                 align: o
                             }]
                         }
                     }
-                    let u = $t(n.parser, s, gn(n.envName)),
-                        f = Math.max(0, ...u.body.map(b => b.length));
-                    return u.cols = new Array(f).fill({
+                    let u = $t(n.parser, s, bn(n.envName)),
+                        p = Math.max(0, ...u.body.map(b => b.length));
+                    return u.cols = new Array(p).fill({
                         type: "align",
                         align: o
                     }), t ? {
                         type: "leftright",
                         mode: n.mode,
                         body: [u],
                         left: t[0],
@@ -12064,30 +12064,30 @@
             }), wt({
                 type: "array",
                 names: ["subarray"],
                 props: {
                     numArgs: 1
                 },
                 handler(n, t) {
-                    let u = (Jr(t[0]) ? [t[0]] : de(t[0], "ordgroup").body).map(function(b) {
-                        let S = rn(b).text;
+                    let u = (Kr(t[0]) ? [t[0]] : de(t[0], "ordgroup").body).map(function(b) {
+                        let S = nn(b).text;
                         if ("lc".indexOf(S) !== -1) return {
                             type: "align",
                             align: S
                         };
                         throw new a("Unknown column alignment: " + S, b)
                     });
                     if (u.length > 1) throw new a("{subarray} can contain only one column");
-                    let f = {
+                    let p = {
                         cols: u,
                         hskipBeforeAndAfter: !1,
                         arraystretch: .5
                     };
-                    if (f = $t(n.parser, f, "script"), f.body.length > 0 && f.body[0].length > 1) throw new a("{subarray} can contain only one column");
-                    return f
+                    if (p = $t(n.parser, p, "script"), p.body.length > 0 && p.body[0].length > 1) throw new a("{subarray} can contain only one column");
+                    return p
                 },
                 htmlBuilder: kt,
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["cases", "dcases", "rcases", "drcases"],
                 props: {
@@ -12104,15 +12104,15 @@
                             }, {
                                 type: "align",
                                 align: "l",
                                 pregap: 0,
                                 postgap: 0
                             }]
                         },
-                        o = $t(n.parser, t, gn(n.envName));
+                        o = $t(n.parser, t, bn(n.envName));
                     return {
                         type: "leftright",
                         mode: n.mode,
                         body: [o],
                         left: n.envName.indexOf("r") > -1 ? "." : "\\{",
                         right: n.envName.indexOf("r") > -1 ? "\\}" : ".",
                         rightColor: void 0
@@ -12122,59 +12122,59 @@
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["align", "align*", "aligned", "split"],
                 props: {
                     numArgs: 0
                 },
-                handler: yo,
+                handler: ko,
                 htmlBuilder: kt,
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["gathered", "gather", "gather*"],
                 props: {
                     numArgs: 0
                 },
                 handler(n) {
-                    R.contains(["gather", "gather*"], n.envName) && n0(n);
+                    R.contains(["gather", "gather*"], n.envName) && i0(n);
                     let t = {
                         cols: [{
                             type: "align",
                             align: "c"
                         }],
                         addJot: !0,
                         colSeparationType: "gather",
-                        autoTag: fn(n.envName),
+                        autoTag: gn(n.envName),
                         emptySingleRow: !0,
                         leqno: n.parser.settings.leqno
                     };
                     return $t(n.parser, t, "display")
                 },
                 htmlBuilder: kt,
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["alignat", "alignat*", "alignedat"],
                 props: {
                     numArgs: 1
                 },
-                handler: yo,
+                handler: ko,
                 htmlBuilder: kt,
                 mathmlBuilder: _t
             }), wt({
                 type: "array",
                 names: ["equation", "equation*"],
                 props: {
                     numArgs: 0
                 },
                 handler(n) {
-                    n0(n);
+                    i0(n);
                     let t = {
-                        autoTag: fn(n.envName),
+                        autoTag: gn(n.envName),
                         emptySingleRow: !0,
                         singleRow: !0,
                         maxNumCols: 1,
                         leqno: n.parser.settings.leqno
                     };
                     return $t(n.parser, t, "display")
                 },
@@ -12183,265 +12183,265 @@
             }), wt({
                 type: "array",
                 names: ["CD"],
                 props: {
                     numArgs: 0
                 },
                 handler(n) {
-                    return n0(n), k1(n.parser)
+                    return i0(n), _1(n.parser)
                 },
                 htmlBuilder: kt,
                 mathmlBuilder: _t
-            }), w("\\nonumber", "\\gdef\\@eqnsw{0}"), w("\\notag", "\\nonumber"), Z({
+            }), k("\\nonumber", "\\gdef\\@eqnsw{0}"), k("\\notag", "\\nonumber"), Q({
                 type: "text",
                 names: ["\\hline", "\\hdashline"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0,
                     allowedInMath: !0
                 },
                 handler(n, t) {
                     throw new a(n.funcName + " valid only within array environment")
                 }
             });
-            var xo = fo;
-            Z({
+            var _o = xo;
+            Q({
                 type: "environment",
                 names: ["\\begin", "\\end"],
                 props: {
                     numArgs: 1,
                     argTypes: ["text"]
                 },
                 handler(n, t) {
                     let {
                         parser: o,
                         funcName: s
                     } = n, u = t[0];
                     if (u.type !== "ordgroup") throw new a("Invalid environment name", u);
-                    let f = "";
-                    for (let b = 0; b < u.body.length; ++b) f += de(u.body[b], "textord").text;
+                    let p = "";
+                    for (let b = 0; b < u.body.length; ++b) p += de(u.body[b], "textord").text;
                     if (s === "\\begin") {
-                        if (!xo.hasOwnProperty(f)) throw new a("No such environment: " + f, u);
-                        let b = xo[f],
+                        if (!_o.hasOwnProperty(p)) throw new a("No such environment: " + p, u);
+                        let b = _o[p],
                             {
                                 args: v,
                                 optArgs: S
-                            } = o.parseArguments("\\begin{" + f + "}", b),
+                            } = o.parseArguments("\\begin{" + p + "}", b),
                             E = {
                                 mode: o.mode,
-                                envName: f,
+                                envName: p,
                                 parser: o
                             },
                             z = b.handler(E, v, S);
                         o.expect("\\end", !1);
                         let F = o.nextToken,
                             N = de(o.parseFunction(), "environment");
-                        if (N.name !== f) throw new a("Mismatch: \\begin{" + f + "} matched by \\end{" + N.name + "}", F);
+                        if (N.name !== p) throw new a("Mismatch: \\begin{" + p + "} matched by \\end{" + N.name + "}", F);
                         return z
                     }
                     return {
                         type: "environment",
                         mode: o.mode,
-                        name: f,
+                        name: p,
                         nameGroup: u
                     }
                 }
             });
-            let vo = (n, t) => {
+            let So = (n, t) => {
                     let o = n.font,
                         s = t.withFont(o);
                     return ve(n.body, s)
                 },
-                wo = (n, t) => {
+                Co = (n, t) => {
                     let o = n.font,
                         s = t.withFont(o);
                     return Ee(n.body, s)
                 },
-                ko = {
+                To = {
                     "\\Bbb": "\\mathbb",
                     "\\bold": "\\mathbf",
                     "\\frak": "\\mathfrak",
                     "\\bm": "\\boldsymbol"
                 };
-            Z({
+            Q({
                 type: "font",
                 names: ["\\mathrm", "\\mathit", "\\mathbf", "\\mathnormal", "\\mathbb", "\\mathcal", "\\mathfrak", "\\mathscr", "\\mathsf", "\\mathtt", "\\Bbb", "\\bold", "\\frak"],
                 props: {
                     numArgs: 1,
                     allowedInArgument: !0
                 },
                 handler: (n, t) => {
                     let {
                         parser: o,
                         funcName: s
-                    } = n, u = Zr(t[0]), f = s;
-                    return f in ko && (f = ko[f]), {
+                    } = n, u = Xr(t[0]), p = s;
+                    return p in To && (p = To[p]), {
                         type: "font",
                         mode: o.mode,
-                        font: f.slice(1),
+                        font: p.slice(1),
                         body: u
                     }
                 },
-                htmlBuilder: vo,
-                mathmlBuilder: wo
-            }), Z({
+                htmlBuilder: So,
+                mathmlBuilder: Co
+            }), Q({
                 type: "mclass",
                 names: ["\\boldsymbol", "\\bm"],
                 props: {
                     numArgs: 1
                 },
                 handler: (n, t) => {
                     let {
                         parser: o
                     } = n, s = t[0], u = R.isCharacterBox(s);
                     return {
                         type: "mclass",
                         mode: o.mode,
-                        mclass: e0(s),
+                        mclass: t0(s),
                         body: [{
                             type: "font",
                             mode: o.mode,
                             font: "boldsymbol",
                             body: s
                         }],
                         isCharacterBox: u
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "font",
                 names: ["\\rm", "\\sf", "\\tt", "\\bf", "\\it", "\\cal"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0
                 },
                 handler: (n, t) => {
                     let {
                         parser: o,
                         funcName: s,
                         breakOnTokenText: u
                     } = n, {
-                        mode: f
+                        mode: p
                     } = o, b = o.parseExpression(!0, u), v = "math" + s.slice(1);
                     return {
                         type: "font",
-                        mode: f,
+                        mode: p,
                         font: v,
                         body: {
                             type: "ordgroup",
                             mode: o.mode,
                             body: b
                         }
                     }
                 },
-                htmlBuilder: vo,
-                mathmlBuilder: wo
+                htmlBuilder: So,
+                mathmlBuilder: Co
             });
-            let _o = (n, t) => {
+            let Ao = (n, t) => {
                     let o = t;
-                    return n === "display" ? o = o.id >= $.SCRIPT.id ? o.text() : $.DISPLAY : n === "text" && o.size === $.DISPLAY.size ? o = $.TEXT : n === "script" ? o = $.SCRIPT : n === "scriptscript" && (o = $.SCRIPTSCRIPT), o
+                    return n === "display" ? o = o.id >= G.SCRIPT.id ? o.text() : G.DISPLAY : n === "text" && o.size === G.DISPLAY.size ? o = G.TEXT : n === "script" ? o = G.SCRIPT : n === "scriptscript" && (o = G.SCRIPTSCRIPT), o
                 },
-                bn = (n, t) => {
-                    let o = _o(n.size, t.style),
+                yn = (n, t) => {
+                    let o = Ao(n.size, t.style),
                         s = o.fracNum(),
                         u = o.fracDen(),
-                        f;
-                    f = t.havingStyle(s);
-                    let b = ve(n.numer, f, t);
+                        p;
+                    p = t.havingStyle(s);
+                    let b = ve(n.numer, p, t);
                     if (n.continued) {
                         let xe = 8.5 / t.fontMetrics().ptPerEm,
                             ke = 3.5 / t.fontMetrics().ptPerEm;
                         b.height = b.height < xe ? xe : b.height, b.depth = b.depth < ke ? ke : b.depth
                     }
-                    f = t.havingStyle(u);
-                    let v = ve(n.denom, f, t),
+                    p = t.havingStyle(u);
+                    let v = ve(n.denom, p, t),
                         S, E, z;
                     n.hasBarLine ? (n.barSize ? (E = Ie(n.barSize, t), S = B.makeLineSpan("frac-line", t, E)) : S = B.makeLineSpan("frac-line", t), E = S.height, z = S.height) : (S = null, E = 0, z = t.fontMetrics().defaultRuleThickness);
-                    let F, N, O;
-                    o.size === $.DISPLAY.size || n.size === "display" ? (F = t.fontMetrics().num1, E > 0 ? N = 3 * z : N = 7 * z, O = t.fontMetrics().denom1) : (E > 0 ? (F = t.fontMetrics().num2, N = z) : (F = t.fontMetrics().num3, N = 3 * z), O = t.fontMetrics().denom2);
+                    let F, N, H;
+                    o.size === G.DISPLAY.size || n.size === "display" ? (F = t.fontMetrics().num1, E > 0 ? N = 3 * z : N = 7 * z, H = t.fontMetrics().denom1) : (E > 0 ? (F = t.fontMetrics().num2, N = z) : (F = t.fontMetrics().num3, N = 3 * z), H = t.fontMetrics().denom2);
                     let K;
                     if (S) {
                         let xe = t.fontMetrics().axisHeight;
-                        F - b.depth - (xe + .5 * E) < N && (F += N - (F - b.depth - (xe + .5 * E))), xe - .5 * E - (v.height - O) < N && (O += N - (xe - .5 * E - (v.height - O)));
+                        F - b.depth - (xe + .5 * E) < N && (F += N - (F - b.depth - (xe + .5 * E))), xe - .5 * E - (v.height - H) < N && (H += N - (xe - .5 * E - (v.height - H)));
                         let ke = -(xe - .5 * E);
                         K = B.makeVList({
                             positionType: "individualShift",
                             children: [{
                                 type: "elem",
                                 elem: v,
-                                shift: O
+                                shift: H
                             }, {
                                 type: "elem",
                                 elem: S,
                                 shift: ke
                             }, {
                                 type: "elem",
                                 elem: b,
                                 shift: -F
                             }]
                         }, t)
                     } else {
-                        let xe = F - b.depth - (v.height - O);
-                        xe < N && (F += .5 * (N - xe), O += .5 * (N - xe)), K = B.makeVList({
+                        let xe = F - b.depth - (v.height - H);
+                        xe < N && (F += .5 * (N - xe), H += .5 * (N - xe)), K = B.makeVList({
                             positionType: "individualShift",
                             children: [{
                                 type: "elem",
                                 elem: v,
-                                shift: O
+                                shift: H
                             }, {
                                 type: "elem",
                                 elem: b,
                                 shift: -F
                             }]
                         }, t)
                     }
-                    f = t.havingStyle(o), K.height *= f.sizeMultiplier / t.sizeMultiplier, K.depth *= f.sizeMultiplier / t.sizeMultiplier;
+                    p = t.havingStyle(o), K.height *= p.sizeMultiplier / t.sizeMultiplier, K.depth *= p.sizeMultiplier / t.sizeMultiplier;
                     let ie;
-                    o.size === $.DISPLAY.size ? ie = t.fontMetrics().delim1 : o.size === $.SCRIPTSCRIPT.size ? ie = t.havingStyle($.SCRIPT).fontMetrics().delim2 : ie = t.fontMetrics().delim2;
+                    o.size === G.DISPLAY.size ? ie = t.fontMetrics().delim1 : o.size === G.SCRIPTSCRIPT.size ? ie = t.havingStyle(G.SCRIPT).fontMetrics().delim2 : ie = t.fontMetrics().delim2;
                     let ye, ge;
-                    return n.leftDelim == null ? ye = wr(t, ["mopen"]) : ye = Bt.customSizedDelim(n.leftDelim, ie, !0, t.havingStyle(o), n.mode, ["mopen"]), n.continued ? ge = B.makeSpan([]) : n.rightDelim == null ? ge = wr(t, ["mclose"]) : ge = Bt.customSizedDelim(n.rightDelim, ie, !0, t.havingStyle(o), n.mode, ["mclose"]), B.makeSpan(["mord"].concat(f.sizingClasses(t)), [ye, B.makeSpan(["mfrac"], [K]), ge], t)
+                    return n.leftDelim == null ? ye = wr(t, ["mopen"]) : ye = Bt.customSizedDelim(n.leftDelim, ie, !0, t.havingStyle(o), n.mode, ["mopen"]), n.continued ? ge = B.makeSpan([]) : n.rightDelim == null ? ge = wr(t, ["mclose"]) : ge = Bt.customSizedDelim(n.rightDelim, ie, !0, t.havingStyle(o), n.mode, ["mclose"]), B.makeSpan(["mord"].concat(p.sizingClasses(t)), [ye, B.makeSpan(["mfrac"], [K]), ge], t)
                 },
-                yn = (n, t) => {
+                xn = (n, t) => {
                     let o = new V.MathNode("mfrac", [Ee(n.numer, t), Ee(n.denom, t)]);
                     if (!n.hasBarLine) o.setAttribute("linethickness", "0px");
                     else if (n.barSize) {
                         let u = Ie(n.barSize, t);
-                        o.setAttribute("linethickness", Q(u))
+                        o.setAttribute("linethickness", Z(u))
                     }
-                    let s = _o(n.size, t.style);
+                    let s = Ao(n.size, t.style);
                     if (s.size !== t.style.size) {
                         o = new V.MathNode("mstyle", [o]);
-                        let u = s.size === $.DISPLAY.size ? "true" : "false";
+                        let u = s.size === G.DISPLAY.size ? "true" : "false";
                         o.setAttribute("displaystyle", u), o.setAttribute("scriptlevel", "0")
                     }
                     if (n.leftDelim != null || n.rightDelim != null) {
                         let u = [];
                         if (n.leftDelim != null) {
-                            let f = new V.MathNode("mo", [new V.TextNode(n.leftDelim.replace("\\", ""))]);
-                            f.setAttribute("fence", "true"), u.push(f)
+                            let p = new V.MathNode("mo", [new V.TextNode(n.leftDelim.replace("\\", ""))]);
+                            p.setAttribute("fence", "true"), u.push(p)
                         }
                         if (u.push(o), n.rightDelim != null) {
-                            let f = new V.MathNode("mo", [new V.TextNode(n.rightDelim.replace("\\", ""))]);
-                            f.setAttribute("fence", "true"), u.push(f)
+                            let p = new V.MathNode("mo", [new V.TextNode(n.rightDelim.replace("\\", ""))]);
+                            p.setAttribute("fence", "true"), u.push(p)
                         }
-                        return en(u)
+                        return tn(u)
                     }
                     return o
                 };
-            Z({
+            Q({
                 type: "genfrac",
                 names: ["\\dfrac", "\\frac", "\\tfrac", "\\dbinom", "\\binom", "\\tbinom", "\\\\atopfrac", "\\\\bracefrac", "\\\\brackfrac"],
                 props: {
                     numArgs: 2,
                     allowedInArgument: !0
                 },
                 handler: (n, t) => {
                     let {
                         parser: o,
                         funcName: s
-                    } = n, u = t[0], f = t[1], b, v = null, S = null, E = "auto";
+                    } = n, u = t[0], p = t[1], b, v = null, S = null, E = "auto";
                     switch (s) {
                         case "\\dfrac":
                         case "\\frac":
                         case "\\tfrac":
                             b = !0;
                             break;
                         case "\\\\atopfrac":
@@ -12472,49 +12472,49 @@
                             break
                     }
                     return {
                         type: "genfrac",
                         mode: o.mode,
                         continued: !1,
                         numer: u,
-                        denom: f,
+                        denom: p,
                         hasBarLine: b,
                         leftDelim: v,
                         rightDelim: S,
                         size: E,
                         barSize: null
                     }
                 },
-                htmlBuilder: bn,
-                mathmlBuilder: yn
-            }), Z({
+                htmlBuilder: yn,
+                mathmlBuilder: xn
+            }), Q({
                 type: "genfrac",
                 names: ["\\cfrac"],
                 props: {
                     numArgs: 2
                 },
                 handler: (n, t) => {
                     let {
                         parser: o,
                         funcName: s
-                    } = n, u = t[0], f = t[1];
+                    } = n, u = t[0], p = t[1];
                     return {
                         type: "genfrac",
                         mode: o.mode,
                         continued: !0,
                         numer: u,
-                        denom: f,
+                        denom: p,
                         hasBarLine: !0,
                         leftDelim: null,
                         rightDelim: null,
                         size: "display",
                         barSize: null
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "infix",
                 names: ["\\over", "\\choose", "\\atop", "\\brace", "\\brack"],
                 props: {
                     numArgs: 0,
                     infix: !0
                 },
                 handler(n) {
@@ -12546,56 +12546,56 @@
                         type: "infix",
                         mode: t.mode,
                         replaceWith: u,
                         token: s
                     }
                 }
             });
-            let So = ["display", "text", "script", "scriptscript"],
-                Co = function(n) {
+            let qo = ["display", "text", "script", "scriptscript"],
+                Mo = function(n) {
                     let t = null;
                     return n.length > 0 && (t = n, t = t === "." ? null : t), t
                 };
-            Z({
+            Q({
                 type: "genfrac",
                 names: ["\\genfrac"],
                 props: {
                     numArgs: 6,
                     allowedInArgument: !0,
                     argTypes: ["math", "math", "size", "text", "math", "math"]
                 },
                 handler(n, t) {
                     let {
                         parser: o
-                    } = n, s = t[4], u = t[5], f = Zr(t[0]), b = f.type === "atom" && f.family === "open" ? Co(f.text) : null, v = Zr(t[1]), S = v.type === "atom" && v.family === "close" ? Co(v.text) : null, E = de(t[2], "size"), z, F = null;
+                    } = n, s = t[4], u = t[5], p = Xr(t[0]), b = p.type === "atom" && p.family === "open" ? Mo(p.text) : null, v = Xr(t[1]), S = v.type === "atom" && v.family === "close" ? Mo(v.text) : null, E = de(t[2], "size"), z, F = null;
                     E.isBlank ? z = !0 : (F = E.value, z = F.number > 0);
                     let N = "auto",
-                        O = t[3];
-                    if (O.type === "ordgroup") {
-                        if (O.body.length > 0) {
-                            let K = de(O.body[0], "textord");
-                            N = So[Number(K.text)]
+                        H = t[3];
+                    if (H.type === "ordgroup") {
+                        if (H.body.length > 0) {
+                            let K = de(H.body[0], "textord");
+                            N = qo[Number(K.text)]
                         }
-                    } else O = de(O, "textord"), N = So[Number(O.text)];
+                    } else H = de(H, "textord"), N = qo[Number(H.text)];
                     return {
                         type: "genfrac",
                         mode: o.mode,
                         numer: s,
                         denom: u,
                         continued: !1,
                         hasBarLine: z,
                         barSize: F,
                         leftDelim: b,
                         rightDelim: S,
                         size: N
                     }
                 },
-                htmlBuilder: bn,
-                mathmlBuilder: yn
-            }), Z({
+                htmlBuilder: yn,
+                mathmlBuilder: xn
+            }), Q({
                 type: "infix",
                 names: ["\\above"],
                 props: {
                     numArgs: 1,
                     argTypes: ["size"],
                     infix: !0
                 },
@@ -12609,73 +12609,73 @@
                         type: "infix",
                         mode: o.mode,
                         replaceWith: "\\\\abovefrac",
                         size: de(t[0], "size").value,
                         token: u
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "genfrac",
                 names: ["\\\\abovefrac"],
                 props: {
                     numArgs: 3,
                     argTypes: ["math", "size", "math"]
                 },
                 handler: (n, t) => {
                     let {
                         parser: o,
                         funcName: s
-                    } = n, u = t[0], f = A(de(t[1], "infix").size), b = t[2], v = f.number > 0;
+                    } = n, u = t[0], p = A(de(t[1], "infix").size), b = t[2], v = p.number > 0;
                     return {
                         type: "genfrac",
                         mode: o.mode,
                         numer: u,
                         denom: b,
                         continued: !1,
                         hasBarLine: v,
-                        barSize: f,
+                        barSize: p,
                         leftDelim: null,
                         rightDelim: null,
                         size: "auto"
                     }
                 },
-                htmlBuilder: bn,
-                mathmlBuilder: yn
+                htmlBuilder: yn,
+                mathmlBuilder: xn
             });
-            let To = (n, t) => {
+            let Eo = (n, t) => {
                 let o = t.style,
                     s, u;
                 n.type === "supsub" ? (s = n.sup ? ve(n.sup, t.havingStyle(o.sup()), t) : ve(n.sub, t.havingStyle(o.sub()), t), u = de(n.base, "horizBrace")) : u = de(n, "horizBrace");
-                let f = ve(u.base, t.havingBaseStyle($.DISPLAY)),
+                let p = ve(u.base, t.havingBaseStyle(G.DISPLAY)),
                     b = Ft.svgSpan(u, t),
                     v;
                 if (u.isOver ? (v = B.makeVList({
                         positionType: "firstBaseline",
                         children: [{
                             type: "elem",
-                            elem: f
+                            elem: p
                         }, {
                             type: "kern",
                             size: .1
                         }, {
                             type: "elem",
                             elem: b
                         }]
                     }, t), v.children[0].children[0].children[1].classes.push("svg-align")) : (v = B.makeVList({
                         positionType: "bottom",
-                        positionData: f.depth + .1 + b.height,
+                        positionData: p.depth + .1 + b.height,
                         children: [{
                             type: "elem",
                             elem: b
                         }, {
                             type: "kern",
                             size: .1
                         }, {
                             type: "elem",
-                            elem: f
+                            elem: p
                         }]
                     }, t), v.children[0].children[0].children[0].classes.push("svg-align")), s) {
                     let S = B.makeSpan(["mord", u.isOver ? "mover" : "munder"], [v], t);
                     u.isOver ? v = B.makeVList({
                         positionType: "firstBaseline",
                         children: [{
                             type: "elem",
@@ -12700,15 +12700,15 @@
                             type: "elem",
                             elem: S
                         }]
                     }, t)
                 }
                 return B.makeSpan(["mord", u.isOver ? "mover" : "munder"], [v], t)
             };
-            Z({
+            Q({
                 type: "horizBrace",
                 names: ["\\overbrace", "\\underbrace"],
                 props: {
                     numArgs: 1
                 },
                 handler(n, t) {
                     let {
@@ -12719,20 +12719,20 @@
                         type: "horizBrace",
                         mode: o.mode,
                         label: s,
                         isOver: /^\\over/.test(s),
                         base: t[0]
                     }
                 },
-                htmlBuilder: To,
+                htmlBuilder: Eo,
                 mathmlBuilder: (n, t) => {
                     let o = Ft.mathMLnode(n.label);
                     return new V.MathNode(n.isOver ? "mover" : "munder", [Ee(n.base, t), o])
                 }
-            }), Z({
+            }), Q({
                 type: "href",
                 names: ["\\href"],
                 props: {
                     numArgs: 2,
                     argTypes: ["url", "original"],
                     allowedInText: !0
                 },
@@ -12747,22 +12747,22 @@
                         type: "href",
                         mode: o.mode,
                         href: u,
                         body: je(s)
                     } : o.formatUnsupportedCmd("\\href")
                 },
                 htmlBuilder: (n, t) => {
-                    let o = Qe(n.body, t, !1);
+                    let o = Ze(n.body, t, !1);
                     return B.makeAnchor(n.href, [], o, t)
                 },
                 mathmlBuilder: (n, t) => {
                     let o = Ht(n.body, t);
                     return o instanceof ht || (o = new ht("mrow", [o])), o.setAttribute("href", n.href), o
                 }
-            }), Z({
+            }), Q({
                 type: "href",
                 names: ["\\url"],
                 props: {
                     numArgs: 1,
                     argTypes: ["url"],
                     allowedInText: !0
                 },
@@ -12779,28 +12779,28 @@
                         let v = s[b];
                         v === "~" && (v = "\\textasciitilde"), u.push({
                             type: "textord",
                             mode: "text",
                             text: v
                         })
                     }
-                    let f = {
+                    let p = {
                         type: "text",
                         mode: o.mode,
                         font: "\\texttt",
                         body: u
                     };
                     return {
                         type: "href",
                         mode: o.mode,
                         href: s,
-                        body: je(f)
+                        body: je(p)
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "hbox",
                 names: ["\\hbox"],
                 props: {
                     numArgs: 1,
                     argTypes: ["text"],
                     allowedInText: !0,
                     primitive: !0
@@ -12812,57 +12812,57 @@
                     return {
                         type: "hbox",
                         mode: o.mode,
                         body: je(t[0])
                     }
                 },
                 htmlBuilder(n, t) {
-                    let o = Qe(n.body, t, !1);
+                    let o = Ze(n.body, t, !1);
                     return B.makeFragment(o)
                 },
                 mathmlBuilder(n, t) {
                     return new V.MathNode("mrow", it(n.body, t))
                 }
-            }), Z({
+            }), Q({
                 type: "html",
                 names: ["\\htmlClass", "\\htmlId", "\\htmlStyle", "\\htmlData"],
                 props: {
                     numArgs: 2,
                     argTypes: ["raw", "original"],
                     allowedInText: !0
                 },
                 handler: (n, t) => {
                     let {
                         parser: o,
                         funcName: s,
                         token: u
-                    } = n, f = de(t[0], "raw").string, b = t[1];
+                    } = n, p = de(t[0], "raw").string, b = t[1];
                     o.settings.strict && o.settings.reportNonstrict("htmlExtension", "HTML extension is disabled on strict mode");
                     let v, S = {};
                     switch (s) {
                         case "\\htmlClass":
-                            S.class = f, v = {
+                            S.class = p, v = {
                                 command: "\\htmlClass",
-                                class: f
+                                class: p
                             };
                             break;
                         case "\\htmlId":
-                            S.id = f, v = {
+                            S.id = p, v = {
                                 command: "\\htmlId",
-                                id: f
+                                id: p
                             };
                             break;
                         case "\\htmlStyle":
-                            S.style = f, v = {
+                            S.style = p, v = {
                                 command: "\\htmlStyle",
-                                style: f
+                                style: p
                             };
                             break;
                         case "\\htmlData": {
-                            let E = f.split(",");
+                            let E = p.split(",");
                             for (let z = 0; z < E.length; z++) {
                                 let F = E[z].split("=");
                                 if (F.length !== 2) throw new a("Error parsing key-value for \\htmlData");
                                 S["data-" + F[0].trim()] = F[1].trim()
                             }
                             v = {
                                 command: "\\htmlData",
@@ -12877,23 +12877,23 @@
                         type: "html",
                         mode: o.mode,
                         attributes: S,
                         body: je(b)
                     } : o.formatUnsupportedCmd(s)
                 },
                 htmlBuilder: (n, t) => {
-                    let o = Qe(n.body, t, !1),
+                    let o = Ze(n.body, t, !1),
                         s = ["enclosing"];
                     n.attributes.class && s.push(...n.attributes.class.trim().split(/\s+/));
                     let u = B.makeSpan(s, o, t);
-                    for (let f in n.attributes) f !== "class" && n.attributes.hasOwnProperty(f) && u.setAttribute(f, n.attributes[f]);
+                    for (let p in n.attributes) p !== "class" && n.attributes.hasOwnProperty(p) && u.setAttribute(p, n.attributes[p]);
                     return u
                 },
                 mathmlBuilder: (n, t) => Ht(n.body, t)
-            }), Z({
+            }), Q({
                 type: "htmlmathml",
                 names: ["\\html@mathml"],
                 props: {
                     numArgs: 2,
                     allowedInText: !0
                 },
                 handler: (n, t) => {
@@ -12904,75 +12904,75 @@
                         type: "htmlmathml",
                         mode: o.mode,
                         html: je(t[0]),
                         mathml: je(t[1])
                     }
                 },
                 htmlBuilder: (n, t) => {
-                    let o = Qe(n.html, t, !1);
+                    let o = Ze(n.html, t, !1);
                     return B.makeFragment(o)
                 },
                 mathmlBuilder: (n, t) => Ht(n.mathml, t)
             });
-            let xn = function(n) {
+            let vn = function(n) {
                 if (/^[-+]? *(\d+(\.\d*)?|\.\d+)$/.test(n)) return {
                     number: +n,
                     unit: "bp"
                 };
                 {
                     let t = /([-+]?) *(\d+(?:\.\d*)?|\.\d+) *([a-z]{2})/.exec(n);
                     if (!t) throw new a("Invalid size: '" + n + "' in \\includegraphics");
                     let o = {
                         number: +(t[1] + t[2]),
                         unit: t[3]
                     };
-                    if (!Ei(o)) throw new a("Invalid unit: '" + o.unit + "' in \\includegraphics.");
+                    if (!Fi(o)) throw new a("Invalid unit: '" + o.unit + "' in \\includegraphics.");
                     return o
                 }
             };
-            Z({
+            Q({
                 type: "includegraphics",
                 names: ["\\includegraphics"],
                 props: {
                     numArgs: 1,
                     numOptionalArgs: 1,
                     argTypes: ["raw", "url"],
                     allowedInText: !1
                 },
                 handler: (n, t, o) => {
                     let {
                         parser: s
                     } = n, u = {
                         number: 0,
                         unit: "em"
-                    }, f = {
+                    }, p = {
                         number: .9,
                         unit: "em"
                     }, b = {
                         number: 0,
                         unit: "em"
                     }, v = "";
                     if (o[0]) {
                         let z = de(o[0], "raw").string.split(",");
                         for (let F = 0; F < z.length; F++) {
                             let N = z[F].split("=");
                             if (N.length === 2) {
-                                let O = N[1].trim();
+                                let H = N[1].trim();
                                 switch (N[0].trim()) {
                                     case "alt":
-                                        v = O;
+                                        v = H;
                                         break;
                                     case "width":
-                                        u = xn(O);
+                                        u = vn(H);
                                         break;
                                     case "height":
-                                        f = xn(O);
+                                        p = vn(H);
                                         break;
                                     case "totalheight":
-                                        b = xn(O);
+                                        b = vn(H);
                                         break;
                                     default:
                                         throw new a("Invalid key: '" + N[0] + "' in \\includegraphics.")
                                 }
                             }
                         }
                     }
@@ -12981,76 +12981,76 @@
                         command: "\\includegraphics",
                         url: S
                     }) ? {
                         type: "includegraphics",
                         mode: s.mode,
                         alt: v,
                         width: u,
-                        height: f,
+                        height: p,
                         totalheight: b,
                         src: S
                     } : s.formatUnsupportedCmd("\\includegraphics")
                 },
                 htmlBuilder: (n, t) => {
                     let o = Ie(n.height, t),
                         s = 0;
                     n.totalheight.number > 0 && (s = Ie(n.totalheight, t) - o);
                     let u = 0;
                     n.width.number > 0 && (u = Ie(n.width, t));
-                    let f = {
-                        height: Q(o + s)
+                    let p = {
+                        height: Z(o + s)
                     };
-                    u > 0 && (f.width = Q(u)), s > 0 && (f.verticalAlign = Q(-s));
-                    let b = new Hu(n.src, n.alt, f);
+                    u > 0 && (p.width = Z(u)), s > 0 && (p.verticalAlign = Z(-s));
+                    let b = new $u(n.src, n.alt, p);
                     return b.height = o, b.depth = s, b
                 },
                 mathmlBuilder: (n, t) => {
                     let o = new V.MathNode("mglyph", []);
                     o.setAttribute("alt", n.alt);
                     let s = Ie(n.height, t),
                         u = 0;
-                    if (n.totalheight.number > 0 && (u = Ie(n.totalheight, t) - s, o.setAttribute("valign", Q(-u))), o.setAttribute("height", Q(s + u)), n.width.number > 0) {
-                        let f = Ie(n.width, t);
-                        o.setAttribute("width", Q(f))
+                    if (n.totalheight.number > 0 && (u = Ie(n.totalheight, t) - s, o.setAttribute("valign", Z(-u))), o.setAttribute("height", Z(s + u)), n.width.number > 0) {
+                        let p = Ie(n.width, t);
+                        o.setAttribute("width", Z(p))
                     }
                     return o.setAttribute("src", n.src), o
                 }
-            }), Z({
+            }), Q({
                 type: "kern",
                 names: ["\\kern", "\\mkern", "\\hskip", "\\mskip"],
                 props: {
                     numArgs: 1,
                     argTypes: ["size"],
                     primitive: !0,
                     allowedInText: !0
                 },
                 handler(n, t) {
                     let {
                         parser: o,
                         funcName: s
                     } = n, u = de(t[0], "size");
                     if (o.settings.strict) {
-                        let f = s[1] === "m",
+                        let p = s[1] === "m",
                             b = u.value.unit === "mu";
-                        f ? (b || o.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + s + " supports only mu units, " + ("not " + u.value.unit + " units")), o.mode !== "math" && o.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + s + " works only in math mode")) : b && o.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + s + " doesn't support mu units")
+                        p ? (b || o.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + s + " supports only mu units, " + ("not " + u.value.unit + " units")), o.mode !== "math" && o.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + s + " works only in math mode")) : b && o.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + s + " doesn't support mu units")
                     }
                     return {
                         type: "kern",
                         mode: o.mode,
                         dimension: u.value
                     }
                 },
                 htmlBuilder(n, t) {
                     return B.makeGlue(n.dimension, t)
                 },
                 mathmlBuilder(n, t) {
                     let o = Ie(n.dimension, t);
                     return new V.SpaceNode(o)
                 }
-            }), Z({
+            }), Q({
                 type: "lap",
                 names: ["\\mathllap", "\\mathrlap", "\\mathclap"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0
                 },
                 handler: (n, t) => {
@@ -13066,75 +13066,75 @@
                     }
                 },
                 htmlBuilder: (n, t) => {
                     let o;
                     n.alignment === "clap" ? (o = B.makeSpan([], [ve(n.body, t)]), o = B.makeSpan(["inner"], [o], t)) : o = B.makeSpan(["inner"], [ve(n.body, t)]);
                     let s = B.makeSpan(["fix"], []),
                         u = B.makeSpan([n.alignment], [o, s], t),
-                        f = B.makeSpan(["strut"]);
-                    return f.style.height = Q(u.height + u.depth), u.depth && (f.style.verticalAlign = Q(-u.depth)), u.children.unshift(f), u = B.makeSpan(["thinbox"], [u], t), B.makeSpan(["mord", "vbox"], [u], t)
+                        p = B.makeSpan(["strut"]);
+                    return p.style.height = Z(u.height + u.depth), u.depth && (p.style.verticalAlign = Z(-u.depth)), u.children.unshift(p), u = B.makeSpan(["thinbox"], [u], t), B.makeSpan(["mord", "vbox"], [u], t)
                 },
                 mathmlBuilder: (n, t) => {
                     let o = new V.MathNode("mpadded", [Ee(n.body, t)]);
                     if (n.alignment !== "rlap") {
                         let s = n.alignment === "llap" ? "-1" : "-0.5";
                         o.setAttribute("lspace", s + "width")
                     }
                     return o.setAttribute("width", "0px"), o
                 }
-            }), Z({
+            }), Q({
                 type: "styling",
                 names: ["\\(", "$"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0,
                     allowedInMath: !1
                 },
                 handler(n, t) {
                     let {
                         funcName: o,
                         parser: s
                     } = n, u = s.mode;
                     s.switchMode("math");
-                    let f = o === "\\(" ? "\\)" : "$",
-                        b = s.parseExpression(!1, f);
-                    return s.expect(f), s.switchMode(u), {
+                    let p = o === "\\(" ? "\\)" : "$",
+                        b = s.parseExpression(!1, p);
+                    return s.expect(p), s.switchMode(u), {
                         type: "styling",
                         mode: s.mode,
                         style: "text",
                         body: b
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "text",
                 names: ["\\)", "\\]"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0,
                     allowedInMath: !1
                 },
                 handler(n, t) {
                     throw new a("Mismatched " + n.funcName)
                 }
             });
-            let Ao = (n, t) => {
+            let Do = (n, t) => {
                 switch (t.style.size) {
-                    case $.DISPLAY.size:
+                    case G.DISPLAY.size:
                         return n.display;
-                    case $.TEXT.size:
+                    case G.TEXT.size:
                         return n.text;
-                    case $.SCRIPT.size:
+                    case G.SCRIPT.size:
                         return n.script;
-                    case $.SCRIPTSCRIPT.size:
+                    case G.SCRIPTSCRIPT.size:
                         return n.scriptscript;
                     default:
                         return n.text
                 }
             };
-            Z({
+            Q({
                 type: "mathchoice",
                 names: ["\\mathchoice"],
                 props: {
                     numArgs: 4,
                     primitive: !0
                 },
                 handler: (n, t) => {
@@ -13147,24 +13147,24 @@
                         display: je(t[0]),
                         text: je(t[1]),
                         script: je(t[2]),
                         scriptscript: je(t[3])
                     }
                 },
                 htmlBuilder: (n, t) => {
-                    let o = Ao(n, t),
-                        s = Qe(o, t, !1);
+                    let o = Do(n, t),
+                        s = Ze(o, t, !1);
                     return B.makeFragment(s)
                 },
                 mathmlBuilder: (n, t) => {
-                    let o = Ao(n, t);
+                    let o = Do(n, t);
                     return Ht(o, t)
                 }
             });
-            let qo = (n, t, o, s, u, f, b) => {
+            let zo = (n, t, o, s, u, p, b) => {
                     n = B.makeSpan([], [n]);
                     let v = o && R.isCharacterBox(o),
                         S, E;
                     if (t) {
                         let N = ve(t, s.havingStyle(u.sup()), s);
                         E = {
                             elem: N,
@@ -13186,28 +13186,28 @@
                             positionData: N,
                             children: [{
                                 type: "kern",
                                 size: s.fontMetrics().bigOpSpacing5
                             }, {
                                 type: "elem",
                                 elem: S.elem,
-                                marginLeft: Q(-f)
+                                marginLeft: Z(-p)
                             }, {
                                 type: "kern",
                                 size: S.kern
                             }, {
                                 type: "elem",
                                 elem: n
                             }, {
                                 type: "kern",
                                 size: E.kern
                             }, {
                                 type: "elem",
                                 elem: E.elem,
-                                marginLeft: Q(f)
+                                marginLeft: Z(p)
                             }, {
                                 type: "kern",
                                 size: s.fontMetrics().bigOpSpacing5
                             }]
                         }, s)
                     } else if (S) {
                         let N = n.height - b;
@@ -13216,15 +13216,15 @@
                             positionData: N,
                             children: [{
                                 type: "kern",
                                 size: s.fontMetrics().bigOpSpacing5
                             }, {
                                 type: "elem",
                                 elem: S.elem,
-                                marginLeft: Q(-f)
+                                marginLeft: Z(-p)
                             }, {
                                 type: "kern",
                                 size: S.kern
                             }, {
                                 type: "elem",
                                 elem: n
                             }]
@@ -13239,116 +13239,116 @@
                                 elem: n
                             }, {
                                 type: "kern",
                                 size: E.kern
                             }, {
                                 type: "elem",
                                 elem: E.elem,
-                                marginLeft: Q(f)
+                                marginLeft: Z(p)
                             }, {
                                 type: "kern",
                                 size: s.fontMetrics().bigOpSpacing5
                             }]
                         }, s)
                     } else return n;
                     let F = [z];
-                    if (S && f !== 0 && !v) {
+                    if (S && p !== 0 && !v) {
                         let N = B.makeSpan(["mspace"], [], s);
-                        N.style.marginRight = Q(f), F.unshift(N)
+                        N.style.marginRight = Z(p), F.unshift(N)
                     }
                     return B.makeSpan(["mop", "op-limits"], F, s)
                 },
-                Mo = ["\\smallint"],
-                sr = (n, t) => {
+                Ro = ["\\smallint"],
+                lr = (n, t) => {
                     let o, s, u = !1,
-                        f;
-                    n.type === "supsub" ? (o = n.sup, s = n.sub, f = de(n.base, "op"), u = !0) : f = de(n, "op");
+                        p;
+                    n.type === "supsub" ? (o = n.sup, s = n.sub, p = de(n.base, "op"), u = !0) : p = de(n, "op");
                     let b = t.style,
                         v = !1;
-                    b.size === $.DISPLAY.size && f.symbol && !R.contains(Mo, f.name) && (v = !0);
+                    b.size === G.DISPLAY.size && p.symbol && !R.contains(Ro, p.name) && (v = !0);
                     let S;
-                    if (f.symbol) {
+                    if (p.symbol) {
                         let F = v ? "Size2-Regular" : "Size1-Regular",
                             N = "";
-                        if ((f.name === "\\oiint" || f.name === "\\oiiint") && (N = f.name.slice(1), f.name = N === "oiint" ? "\\iint" : "\\iiint"), S = B.makeSymbol(f.name, F, "math", t, ["mop", "op-symbol", v ? "large-op" : "small-op"]), N.length > 0) {
-                            let O = S.italic,
+                        if ((p.name === "\\oiint" || p.name === "\\oiiint") && (N = p.name.slice(1), p.name = N === "oiint" ? "\\iint" : "\\iiint"), S = B.makeSymbol(p.name, F, "math", t, ["mop", "op-symbol", v ? "large-op" : "small-op"]), N.length > 0) {
+                            let H = S.italic,
                                 K = B.staticSvg(N + "Size" + (v ? "2" : "1"), t);
                             S = B.makeVList({
                                 positionType: "individualShift",
                                 children: [{
                                     type: "elem",
                                     elem: S,
                                     shift: 0
                                 }, {
                                     type: "elem",
                                     elem: K,
                                     shift: v ? .08 : 0
                                 }]
-                            }, t), f.name = "\\" + N, S.classes.unshift("mop"), S.italic = O
+                            }, t), p.name = "\\" + N, S.classes.unshift("mop"), S.italic = H
                         }
-                    } else if (f.body) {
-                        let F = Qe(f.body, t, !0);
+                    } else if (p.body) {
+                        let F = Ze(p.body, t, !0);
                         F.length === 1 && F[0] instanceof ut ? (S = F[0], S.classes[0] = "mop") : S = B.makeSpan(["mop"], F, t)
                     } else {
                         let F = [];
-                        for (let N = 1; N < f.name.length; N++) F.push(B.mathsym(f.name[N], f.mode, t));
+                        for (let N = 1; N < p.name.length; N++) F.push(B.mathsym(p.name[N], p.mode, t));
                         S = B.makeSpan(["mop"], F, t)
                     }
                     let E = 0,
                         z = 0;
-                    return (S instanceof ut || f.name === "\\oiint" || f.name === "\\oiiint") && !f.suppressBaseShift && (E = (S.height - S.depth) / 2 - t.fontMetrics().axisHeight, z = S.italic), u ? qo(S, o, s, t, b, z, E) : (E && (S.style.position = "relative", S.style.top = Q(E)), S)
+                    return (S instanceof ut || p.name === "\\oiint" || p.name === "\\oiiint") && !p.suppressBaseShift && (E = (S.height - S.depth) / 2 - t.fontMetrics().axisHeight, z = S.italic), u ? zo(S, o, s, t, b, z, E) : (E && (S.style.position = "relative", S.style.top = Z(E)), S)
                 },
                 Cr = (n, t) => {
                     let o;
-                    if (n.symbol) o = new ht("mo", [dt(n.name, n.mode)]), R.contains(Mo, n.name) && o.setAttribute("largeop", "false");
+                    if (n.symbol) o = new ht("mo", [dt(n.name, n.mode)]), R.contains(Ro, n.name) && o.setAttribute("largeop", "false");
                     else if (n.body) o = new ht("mo", it(n.body, t));
                     else {
                         o = new ht("mi", [new kr(n.name.slice(1))]);
                         let s = new ht("mo", [dt("\u2061", "text")]);
-                        n.parentIsSupSub ? o = new ht("mrow", [o, s]) : o = ji([o, s])
+                        n.parentIsSupSub ? o = new ht("mrow", [o, s]) : o = Zi([o, s])
                     }
                     return o
                 },
-                N1 = {
+                L1 = {
                     "\u220F": "\\prod",
                     "\u2210": "\\coprod",
                     "\u2211": "\\sum",
                     "\u22C0": "\\bigwedge",
                     "\u22C1": "\\bigvee",
                     "\u22C2": "\\bigcap",
                     "\u22C3": "\\bigcup",
                     "\u2A00": "\\bigodot",
                     "\u2A01": "\\bigoplus",
                     "\u2A02": "\\bigotimes",
                     "\u2A04": "\\biguplus",
                     "\u2A06": "\\bigsqcup"
                 };
-            Z({
+            Q({
                 type: "op",
                 names: ["\\coprod", "\\bigvee", "\\bigwedge", "\\biguplus", "\\bigcap", "\\bigcup", "\\intop", "\\prod", "\\sum", "\\bigotimes", "\\bigoplus", "\\bigodot", "\\bigsqcup", "\\smallint", "\u220F", "\u2210", "\u2211", "\u22C0", "\u22C1", "\u22C2", "\u22C3", "\u2A00", "\u2A01", "\u2A02", "\u2A04", "\u2A06"],
                 props: {
                     numArgs: 0
                 },
                 handler: (n, t) => {
                     let {
                         parser: o,
                         funcName: s
                     } = n, u = s;
-                    return u.length === 1 && (u = N1[u]), {
+                    return u.length === 1 && (u = L1[u]), {
                         type: "op",
                         mode: o.mode,
                         limits: !0,
                         parentIsSupSub: !1,
                         symbol: !0,
                         name: u
                     }
                 },
-                htmlBuilder: sr,
+                htmlBuilder: lr,
                 mathmlBuilder: Cr
-            }), Z({
+            }), Q({
                 type: "op",
                 names: ["\\mathop"],
                 props: {
                     numArgs: 1,
                     primitive: !0
                 },
                 handler: (n, t) => {
@@ -13360,26 +13360,26 @@
                         mode: o.mode,
                         limits: !1,
                         parentIsSupSub: !1,
                         symbol: !1,
                         body: je(s)
                     }
                 },
-                htmlBuilder: sr,
+                htmlBuilder: lr,
                 mathmlBuilder: Cr
             });
-            let L1 = {
+            let P1 = {
                 "\u222B": "\\int",
                 "\u222C": "\\iint",
                 "\u222D": "\\iiint",
                 "\u222E": "\\oint",
                 "\u222F": "\\oiint",
                 "\u2230": "\\oiiint"
             };
-            Z({
+            Q({
                 type: "op",
                 names: ["\\arcsin", "\\arccos", "\\arctan", "\\arctg", "\\arcctg", "\\arg", "\\ch", "\\cos", "\\cosec", "\\cosh", "\\cot", "\\cotg", "\\coth", "\\csc", "\\ctg", "\\cth", "\\deg", "\\dim", "\\exp", "\\hom", "\\ker", "\\lg", "\\ln", "\\log", "\\sec", "\\sin", "\\sinh", "\\sh", "\\tan", "\\tanh", "\\tg", "\\th"],
                 props: {
                     numArgs: 0
                 },
                 handler(n) {
                     let {
@@ -13391,17 +13391,17 @@
                         mode: t.mode,
                         limits: !1,
                         parentIsSupSub: !1,
                         symbol: !1,
                         name: o
                     }
                 },
-                htmlBuilder: sr,
+                htmlBuilder: lr,
                 mathmlBuilder: Cr
-            }), Z({
+            }), Q({
                 type: "op",
                 names: ["\\det", "\\gcd", "\\inf", "\\lim", "\\max", "\\min", "\\Pr", "\\sup"],
                 props: {
                     numArgs: 0
                 },
                 handler(n) {
                     let {
@@ -13413,63 +13413,63 @@
                         mode: t.mode,
                         limits: !0,
                         parentIsSupSub: !1,
                         symbol: !1,
                         name: o
                     }
                 },
-                htmlBuilder: sr,
+                htmlBuilder: lr,
                 mathmlBuilder: Cr
-            }), Z({
+            }), Q({
                 type: "op",
                 names: ["\\int", "\\iint", "\\iiint", "\\oint", "\\oiint", "\\oiiint", "\u222B", "\u222C", "\u222D", "\u222E", "\u222F", "\u2230"],
                 props: {
                     numArgs: 0
                 },
                 handler(n) {
                     let {
                         parser: t,
                         funcName: o
                     } = n, s = o;
-                    return s.length === 1 && (s = L1[s]), {
+                    return s.length === 1 && (s = P1[s]), {
                         type: "op",
                         mode: t.mode,
                         limits: !1,
                         parentIsSupSub: !1,
                         symbol: !0,
                         name: s
                     }
                 },
-                htmlBuilder: sr,
+                htmlBuilder: lr,
                 mathmlBuilder: Cr
             });
-            let Eo = (n, t) => {
+            let Fo = (n, t) => {
                 let o, s, u = !1,
-                    f;
-                n.type === "supsub" ? (o = n.sup, s = n.sub, f = de(n.base, "operatorname"), u = !0) : f = de(n, "operatorname");
+                    p;
+                n.type === "supsub" ? (o = n.sup, s = n.sub, p = de(n.base, "operatorname"), u = !0) : p = de(n, "operatorname");
                 let b;
-                if (f.body.length > 0) {
-                    let v = f.body.map(E => {
+                if (p.body.length > 0) {
+                    let v = p.body.map(E => {
                             let z = E.text;
                             return typeof z == "string" ? {
                                 type: "textord",
                                 mode: E.mode,
                                 text: z
                             } : E
                         }),
-                        S = Qe(v, t.withFont("mathrm"), !0);
+                        S = Ze(v, t.withFont("mathrm"), !0);
                     for (let E = 0; E < S.length; E++) {
                         let z = S[E];
                         z instanceof ut && (z.text = z.text.replace(/\u2212/, "-").replace(/\u2217/, "*"))
                     }
                     b = B.makeSpan(["mop"], S, t)
                 } else b = B.makeSpan(["mop"], [], t);
-                return u ? qo(b, o, s, t, t.style, 0, 0) : b
+                return u ? zo(b, o, s, t, t.style, 0, 0) : b
             };
-            Z({
+            Q({
                 type: "operatorname",
                 names: ["\\operatorname@", "\\operatornamewithlimits"],
                 props: {
                     numArgs: 1
                 },
                 handler: (n, t) => {
                     let {
@@ -13481,15 +13481,15 @@
                         mode: o.mode,
                         body: je(u),
                         alwaysHandleSupSub: s === "\\operatornamewithlimits",
                         limits: !1,
                         parentIsSupSub: !1
                     }
                 },
-                htmlBuilder: Eo,
+                htmlBuilder: Fo,
                 mathmlBuilder: (n, t) => {
                     let o = it(n.body, t.withFont("mathrm")),
                         s = !0;
                     for (let b = 0; b < o.length; b++) {
                         let v = o[b];
                         if (!(v instanceof V.SpaceNode))
                             if (v instanceof V.MathNode) switch (v.type) {
@@ -13510,26 +13510,26 @@
                     }
                     if (s) {
                         let b = o.map(v => v.toText()).join("");
                         o = [new V.TextNode(b)]
                     }
                     let u = new V.MathNode("mi", o);
                     u.setAttribute("mathvariant", "normal");
-                    let f = new V.MathNode("mo", [dt("\u2061", "text")]);
-                    return n.parentIsSupSub ? new V.MathNode("mrow", [u, f]) : V.newDocumentFragment([u, f])
+                    let p = new V.MathNode("mo", [dt("\u2061", "text")]);
+                    return n.parentIsSupSub ? new V.MathNode("mrow", [u, p]) : V.newDocumentFragment([u, p])
                 }
-            }), w("\\operatorname", "\\@ifstar\\operatornamewithlimits\\operatorname@"), Jt({
+            }), k("\\operatorname", "\\@ifstar\\operatornamewithlimits\\operatorname@"), Kt({
                 type: "ordgroup",
                 htmlBuilder(n, t) {
-                    return n.semisimple ? B.makeFragment(Qe(n.body, t, !1)) : B.makeSpan(["mord"], Qe(n.body, t, !0), t)
+                    return n.semisimple ? B.makeFragment(Ze(n.body, t, !1)) : B.makeSpan(["mord"], Ze(n.body, t, !0), t)
                 },
                 mathmlBuilder(n, t) {
                     return Ht(n.body, t, !0)
                 }
-            }), Z({
+            }), Q({
                 type: "overline",
                 names: ["\\overline"],
                 props: {
                     numArgs: 1
                 },
                 handler(n, t) {
                     let {
@@ -13541,15 +13541,15 @@
                         body: s
                     }
                 },
                 htmlBuilder(n, t) {
                     let o = ve(n.body, t.havingCrampedStyle()),
                         s = B.makeLineSpan("overline-line", t),
                         u = t.fontMetrics().defaultRuleThickness,
-                        f = B.makeVList({
+                        p = B.makeVList({
                             positionType: "firstBaseline",
                             children: [{
                                 type: "elem",
                                 elem: o
                             }, {
                                 type: "kern",
                                 size: 3 * u
@@ -13557,23 +13557,23 @@
                                 type: "elem",
                                 elem: s
                             }, {
                                 type: "kern",
                                 size: u
                             }]
                         }, t);
-                    return B.makeSpan(["mord", "overline"], [f], t)
+                    return B.makeSpan(["mord", "overline"], [p], t)
                 },
                 mathmlBuilder(n, t) {
                     let o = new V.MathNode("mo", [new V.TextNode("\u203E")]);
                     o.setAttribute("stretchy", "true");
                     let s = new V.MathNode("mover", [Ee(n.body, t), o]);
                     return s.setAttribute("accent", "true"), s
                 }
-            }), Z({
+            }), Q({
                 type: "phantom",
                 names: ["\\phantom"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0
                 },
                 handler: (n, t) => {
@@ -13583,22 +13583,22 @@
                     return {
                         type: "phantom",
                         mode: o.mode,
                         body: je(s)
                     }
                 },
                 htmlBuilder: (n, t) => {
-                    let o = Qe(n.body, t.withPhantom(), !1);
+                    let o = Ze(n.body, t.withPhantom(), !1);
                     return B.makeFragment(o)
                 },
                 mathmlBuilder: (n, t) => {
                     let o = it(n.body, t);
                     return new V.MathNode("mphantom", o)
                 }
-            }), Z({
+            }), Q({
                 type: "hphantom",
                 names: ["\\hphantom"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0
                 },
                 handler: (n, t) => {
@@ -13625,15 +13625,15 @@
                 },
                 mathmlBuilder: (n, t) => {
                     let o = it(je(n.body), t),
                         s = new V.MathNode("mphantom", o),
                         u = new V.MathNode("mpadded", [s]);
                     return u.setAttribute("height", "0px"), u.setAttribute("depth", "0px"), u
                 }
-            }), Z({
+            }), Q({
                 type: "vphantom",
                 names: ["\\vphantom"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0
                 },
                 handler: (n, t) => {
@@ -13653,15 +13653,15 @@
                 },
                 mathmlBuilder: (n, t) => {
                     let o = it(je(n.body), t),
                         s = new V.MathNode("mphantom", o),
                         u = new V.MathNode("mpadded", [s]);
                     return u.setAttribute("width", "0px"), u
                 }
-            }), Z({
+            }), Q({
                 type: "raisebox",
                 names: ["\\raisebox"],
                 props: {
                     numArgs: 2,
                     argTypes: ["size", "hbox"],
                     allowedInText: !0
                 },
@@ -13689,15 +13689,15 @@
                     }, t)
                 },
                 mathmlBuilder(n, t) {
                     let o = new V.MathNode("mpadded", [Ee(n.body, t)]),
                         s = n.dy.number + n.dy.unit;
                     return o.setAttribute("voffset", s), o
                 }
-            }), Z({
+            }), Q({
                 type: "internal",
                 names: ["\\relax"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0
                 },
                 handler(n) {
@@ -13705,122 +13705,122 @@
                         parser: t
                     } = n;
                     return {
                         type: "internal",
                         mode: t.mode
                     }
                 }
-            }), Z({
+            }), Q({
                 type: "rule",
                 names: ["\\rule"],
                 props: {
                     numArgs: 2,
                     numOptionalArgs: 1,
                     argTypes: ["size", "size", "size"]
                 },
                 handler(n, t, o) {
                     let {
                         parser: s
-                    } = n, u = o[0], f = de(t[0], "size"), b = de(t[1], "size");
+                    } = n, u = o[0], p = de(t[0], "size"), b = de(t[1], "size");
                     return {
                         type: "rule",
                         mode: s.mode,
                         shift: u && de(u, "size").value,
-                        width: f.value,
+                        width: p.value,
                         height: b.value
                     }
                 },
                 htmlBuilder(n, t) {
                     let o = B.makeSpan(["mord", "rule"], [], t),
                         s = Ie(n.width, t),
                         u = Ie(n.height, t),
-                        f = n.shift ? Ie(n.shift, t) : 0;
-                    return o.style.borderRightWidth = Q(s), o.style.borderTopWidth = Q(u), o.style.bottom = Q(f), o.width = s, o.height = u + f, o.depth = -f, o.maxFontSize = u * 1.125 * t.sizeMultiplier, o
+                        p = n.shift ? Ie(n.shift, t) : 0;
+                    return o.style.borderRightWidth = Z(s), o.style.borderTopWidth = Z(u), o.style.bottom = Z(p), o.width = s, o.height = u + p, o.depth = -p, o.maxFontSize = u * 1.125 * t.sizeMultiplier, o
                 },
                 mathmlBuilder(n, t) {
                     let o = Ie(n.width, t),
                         s = Ie(n.height, t),
                         u = n.shift ? Ie(n.shift, t) : 0,
-                        f = t.color && t.getColor() || "black",
+                        p = t.color && t.getColor() || "black",
                         b = new V.MathNode("mspace");
-                    b.setAttribute("mathbackground", f), b.setAttribute("width", Q(o)), b.setAttribute("height", Q(s));
+                    b.setAttribute("mathbackground", p), b.setAttribute("width", Z(o)), b.setAttribute("height", Z(s));
                     let v = new V.MathNode("mpadded", [b]);
-                    return u >= 0 ? v.setAttribute("height", Q(u)) : (v.setAttribute("height", Q(u)), v.setAttribute("depth", Q(-u))), v.setAttribute("voffset", Q(u)), v
+                    return u >= 0 ? v.setAttribute("height", Z(u)) : (v.setAttribute("height", Z(u)), v.setAttribute("depth", Z(-u))), v.setAttribute("voffset", Z(u)), v
                 }
             });
 
-            function Do(n, t, o) {
-                let s = Qe(n, t, !1),
+            function Bo(n, t, o) {
+                let s = Ze(n, t, !1),
                     u = t.sizeMultiplier / o.sizeMultiplier;
-                for (let f = 0; f < s.length; f++) {
-                    let b = s[f].classes.indexOf("sizing");
-                    b < 0 ? Array.prototype.push.apply(s[f].classes, t.sizingClasses(o)) : s[f].classes[b + 1] === "reset-size" + t.size && (s[f].classes[b + 1] = "reset-size" + o.size), s[f].height *= u, s[f].depth *= u
+                for (let p = 0; p < s.length; p++) {
+                    let b = s[p].classes.indexOf("sizing");
+                    b < 0 ? Array.prototype.push.apply(s[p].classes, t.sizingClasses(o)) : s[p].classes[b + 1] === "reset-size" + t.size && (s[p].classes[b + 1] = "reset-size" + o.size), s[p].height *= u, s[p].depth *= u
                 }
                 return B.makeFragment(s)
             }
-            let zo = ["\\tiny", "\\sixptsize", "\\scriptsize", "\\footnotesize", "\\small", "\\normalsize", "\\large", "\\Large", "\\LARGE", "\\huge", "\\Huge"];
-            Z({
+            let No = ["\\tiny", "\\sixptsize", "\\scriptsize", "\\footnotesize", "\\small", "\\normalsize", "\\large", "\\Large", "\\LARGE", "\\huge", "\\Huge"];
+            Q({
                 type: "sizing",
-                names: zo,
+                names: No,
                 props: {
                     numArgs: 0,
                     allowedInText: !0
                 },
                 handler: (n, t) => {
                     let {
                         breakOnTokenText: o,
                         funcName: s,
                         parser: u
-                    } = n, f = u.parseExpression(!1, o);
+                    } = n, p = u.parseExpression(!1, o);
                     return {
                         type: "sizing",
                         mode: u.mode,
-                        size: zo.indexOf(s) + 1,
-                        body: f
+                        size: No.indexOf(s) + 1,
+                        body: p
                     }
                 },
                 htmlBuilder: (n, t) => {
                     let o = t.havingSize(n.size);
-                    return Do(n.body, o, t)
+                    return Bo(n.body, o, t)
                 },
                 mathmlBuilder: (n, t) => {
                     let o = t.havingSize(n.size),
                         s = it(n.body, o),
                         u = new V.MathNode("mstyle", s);
-                    return u.setAttribute("mathsize", Q(o.sizeMultiplier)), u
+                    return u.setAttribute("mathsize", Z(o.sizeMultiplier)), u
                 }
-            }), Z({
+            }), Q({
                 type: "smash",
                 names: ["\\smash"],
                 props: {
                     numArgs: 1,
                     numOptionalArgs: 1,
                     allowedInText: !0
                 },
                 handler: (n, t, o) => {
                     let {
                         parser: s
-                    } = n, u = !1, f = !1, b = o[0] && de(o[0], "ordgroup");
+                    } = n, u = !1, p = !1, b = o[0] && de(o[0], "ordgroup");
                     if (b) {
                         let S = "";
                         for (let E = 0; E < b.body.length; ++E)
                             if (S = b.body[E].text, S === "t") u = !0;
-                            else if (S === "b") f = !0;
+                            else if (S === "b") p = !0;
                         else {
-                            u = !1, f = !1;
+                            u = !1, p = !1;
                             break
                         }
-                    } else u = !0, f = !0;
+                    } else u = !0, p = !0;
                     let v = t[0];
                     return {
                         type: "smash",
                         mode: s.mode,
                         body: v,
                         smashHeight: u,
-                        smashDepth: f
+                        smashDepth: p
                     }
                 },
                 htmlBuilder: (n, t) => {
                     let o = B.makeSpan([], [ve(n.body, t)]);
                     if (!n.smashHeight && !n.smashDepth) return o;
                     if (n.smashHeight && (o.height = 0, o.children))
                         for (let u = 0; u < o.children.length; u++) o.children[u].height = 0;
@@ -13835,50 +13835,50 @@
                     }, t);
                     return B.makeSpan(["mord"], [s], t)
                 },
                 mathmlBuilder: (n, t) => {
                     let o = new V.MathNode("mpadded", [Ee(n.body, t)]);
                     return n.smashHeight && o.setAttribute("height", "0px"), n.smashDepth && o.setAttribute("depth", "0px"), o
                 }
-            }), Z({
+            }), Q({
                 type: "sqrt",
                 names: ["\\sqrt"],
                 props: {
                     numArgs: 1,
                     numOptionalArgs: 1
                 },
                 handler(n, t, o) {
                     let {
                         parser: s
-                    } = n, u = o[0], f = t[0];
+                    } = n, u = o[0], p = t[0];
                     return {
                         type: "sqrt",
                         mode: s.mode,
-                        body: f,
+                        body: p,
                         index: u
                     }
                 },
                 htmlBuilder(n, t) {
                     let o = ve(n.body, t.havingCrampedStyle());
                     o.height === 0 && (o.height = t.fontMetrics().xHeight), o = B.wrapFragment(o, t);
                     let u = t.fontMetrics().defaultRuleThickness,
-                        f = u;
-                    t.style.id < $.TEXT.id && (f = t.fontMetrics().xHeight);
-                    let b = u + f / 4,
+                        p = u;
+                    t.style.id < G.TEXT.id && (p = t.fontMetrics().xHeight);
+                    let b = u + p / 4,
                         v = o.height + o.depth + b + u,
                         {
                             span: S,
                             ruleWidth: E,
                             advanceWidth: z
                         } = Bt.sqrtImage(v, t),
                         F = S.height - E;
                     F > o.height + o.depth + b && (b = (b + F - o.height - o.depth) / 2);
                     let N = S.height - o.height - b - E;
-                    o.style.paddingLeft = Q(z);
-                    let O = B.makeVList({
+                    o.style.paddingLeft = Z(z);
+                    let H = B.makeVList({
                         positionType: "firstBaseline",
                         children: [{
                             type: "elem",
                             elem: o,
                             wrapperClasses: ["svg-align"]
                         }, {
                             type: "kern",
@@ -13888,122 +13888,122 @@
                             elem: S
                         }, {
                             type: "kern",
                             size: E
                         }]
                     }, t);
                     if (n.index) {
-                        let K = t.havingStyle($.SCRIPTSCRIPT),
+                        let K = t.havingStyle(G.SCRIPTSCRIPT),
                             ie = ve(n.index, K, t),
-                            ye = .6 * (O.height - O.depth),
+                            ye = .6 * (H.height - H.depth),
                             ge = B.makeVList({
                                 positionType: "shift",
                                 positionData: -ye,
                                 children: [{
                                     type: "elem",
                                     elem: ie
                                 }]
                             }, t),
                             xe = B.makeSpan(["root"], [ge]);
-                        return B.makeSpan(["mord", "sqrt"], [xe, O], t)
-                    } else return B.makeSpan(["mord", "sqrt"], [O], t)
+                        return B.makeSpan(["mord", "sqrt"], [xe, H], t)
+                    } else return B.makeSpan(["mord", "sqrt"], [H], t)
                 },
                 mathmlBuilder(n, t) {
                     let {
                         body: o,
                         index: s
                     } = n;
                     return s ? new V.MathNode("mroot", [Ee(o, t), Ee(s, t)]) : new V.MathNode("msqrt", [Ee(o, t)])
                 }
             });
-            let Ro = {
-                display: $.DISPLAY,
-                text: $.TEXT,
-                script: $.SCRIPT,
-                scriptscript: $.SCRIPTSCRIPT
+            let Lo = {
+                display: G.DISPLAY,
+                text: G.TEXT,
+                script: G.SCRIPT,
+                scriptscript: G.SCRIPTSCRIPT
             };
-            Z({
+            Q({
                 type: "styling",
                 names: ["\\displaystyle", "\\textstyle", "\\scriptstyle", "\\scriptscriptstyle"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0,
                     primitive: !0
                 },
                 handler(n, t) {
                     let {
                         breakOnTokenText: o,
                         funcName: s,
                         parser: u
-                    } = n, f = u.parseExpression(!0, o), b = s.slice(1, s.length - 5);
+                    } = n, p = u.parseExpression(!0, o), b = s.slice(1, s.length - 5);
                     return {
                         type: "styling",
                         mode: u.mode,
                         style: b,
-                        body: f
+                        body: p
                     }
                 },
                 htmlBuilder(n, t) {
-                    let o = Ro[n.style],
+                    let o = Lo[n.style],
                         s = t.havingStyle(o).withFont("");
-                    return Do(n.body, s, t)
+                    return Bo(n.body, s, t)
                 },
                 mathmlBuilder(n, t) {
-                    let o = Ro[n.style],
+                    let o = Lo[n.style],
                         s = t.havingStyle(o),
                         u = it(n.body, s),
-                        f = new V.MathNode("mstyle", u),
+                        p = new V.MathNode("mstyle", u),
                         v = {
                             display: ["0", "true"],
                             text: ["0", "false"],
                             script: ["1", "false"],
                             scriptscript: ["2", "false"]
                         } [n.style];
-                    return f.setAttribute("scriptlevel", v[0]), f.setAttribute("displaystyle", v[1]), f
+                    return p.setAttribute("scriptlevel", v[0]), p.setAttribute("displaystyle", v[1]), p
                 }
             });
-            let P1 = function(n, t) {
+            let I1 = function(n, t) {
                 let o = n.base;
-                return o ? o.type === "op" ? o.limits && (t.style.size === $.DISPLAY.size || o.alwaysHandleSupSub) ? sr : null : o.type === "operatorname" ? o.alwaysHandleSupSub && (t.style.size === $.DISPLAY.size || o.limits) ? Eo : null : o.type === "accent" ? R.isCharacterBox(o.base) ? nn : null : o.type === "horizBrace" && !n.sub === o.isOver ? To : null : null
+                return o ? o.type === "op" ? o.limits && (t.style.size === G.DISPLAY.size || o.alwaysHandleSupSub) ? lr : null : o.type === "operatorname" ? o.alwaysHandleSupSub && (t.style.size === G.DISPLAY.size || o.limits) ? Fo : null : o.type === "accent" ? R.isCharacterBox(o.base) ? on : null : o.type === "horizBrace" && !n.sub === o.isOver ? Eo : null : null
             };
-            Jt({
+            Kt({
                 type: "supsub",
                 htmlBuilder(n, t) {
-                    let o = P1(n, t);
+                    let o = I1(n, t);
                     if (o) return o(n, t);
                     let {
                         base: s,
                         sup: u,
-                        sub: f
+                        sub: p
                     } = n, b = ve(s, t), v, S, E = t.fontMetrics(), z = 0, F = 0, N = s && R.isCharacterBox(s);
                     if (u) {
                         let ke = t.havingStyle(t.style.sup());
                         v = ve(u, ke, t), N || (z = b.height - ke.fontMetrics().supDrop * ke.sizeMultiplier / t.sizeMultiplier)
                     }
-                    if (f) {
+                    if (p) {
                         let ke = t.havingStyle(t.style.sub());
-                        S = ve(f, ke, t), N || (F = b.depth + ke.fontMetrics().subDrop * ke.sizeMultiplier / t.sizeMultiplier)
+                        S = ve(p, ke, t), N || (F = b.depth + ke.fontMetrics().subDrop * ke.sizeMultiplier / t.sizeMultiplier)
                     }
-                    let O;
-                    t.style === $.DISPLAY ? O = E.sup1 : t.style.cramped ? O = E.sup3 : O = E.sup2;
+                    let H;
+                    t.style === G.DISPLAY ? H = E.sup1 : t.style.cramped ? H = E.sup3 : H = E.sup2;
                     let K = t.sizeMultiplier,
-                        ie = Q(.5 / E.ptPerEm / K),
+                        ie = Z(.5 / E.ptPerEm / K),
                         ye = null;
                     if (S) {
                         let ke = n.base && n.base.type === "op" && n.base.name && (n.base.name === "\\oiint" || n.base.name === "\\oiiint");
-                        (b instanceof ut || ke) && (ye = Q(-b.italic))
+                        (b instanceof ut || ke) && (ye = Z(-b.italic))
                     }
                     let ge;
                     if (v && S) {
-                        z = Math.max(z, O, v.depth + .25 * E.xHeight), F = Math.max(F, E.sub2);
+                        z = Math.max(z, H, v.depth + .25 * E.xHeight), F = Math.max(F, E.sub2);
                         let ze = 4 * E.defaultRuleThickness;
                         if (z - v.depth - (S.height - F) < ze) {
                             F = ze - (z - v.depth) + S.height;
-                            let Ze = .8 * E.xHeight - (z - v.depth);
-                            Ze > 0 && (z += Ze, F -= Ze)
+                            let Qe = .8 * E.xHeight - (z - v.depth);
+                            Qe > 0 && (z += Qe, F -= Qe)
                         }
                         let tt = [{
                             type: "elem",
                             elem: S,
                             shift: F,
                             marginRight: ie,
                             marginLeft: ye
@@ -14026,160 +14026,160 @@
                             marginRight: ie
                         }];
                         ge = B.makeVList({
                             positionType: "shift",
                             positionData: F,
                             children: ke
                         }, t)
-                    } else if (v) z = Math.max(z, O, v.depth + .25 * E.xHeight), ge = B.makeVList({
+                    } else if (v) z = Math.max(z, H, v.depth + .25 * E.xHeight), ge = B.makeVList({
                         positionType: "shift",
                         positionData: -z,
                         children: [{
                             type: "elem",
                             elem: v,
                             marginRight: ie
                         }]
                     }, t);
                     else throw new Error("supsub must have either sup or sub.");
-                    let xe = J0(b, "right") || "mord";
+                    let xe = K0(b, "right") || "mord";
                     return B.makeSpan([xe], [b, B.makeSpan(["msupsub"], [ge])], t)
                 },
                 mathmlBuilder(n, t) {
                     let o = !1,
                         s, u;
                     n.base && n.base.type === "horizBrace" && (u = !!n.sup, u === n.base.isOver && (o = !0, s = n.base.isOver)), n.base && (n.base.type === "op" || n.base.type === "operatorname") && (n.base.parentIsSupSub = !0);
-                    let f = [Ee(n.base, t)];
-                    n.sub && f.push(Ee(n.sub, t)), n.sup && f.push(Ee(n.sup, t));
+                    let p = [Ee(n.base, t)];
+                    n.sub && p.push(Ee(n.sub, t)), n.sup && p.push(Ee(n.sup, t));
                     let b;
                     if (o) b = s ? "mover" : "munder";
                     else if (n.sub)
                         if (n.sup) {
                             let v = n.base;
-                            v && v.type === "op" && v.limits && t.style === $.DISPLAY || v && v.type === "operatorname" && v.alwaysHandleSupSub && (t.style === $.DISPLAY || v.limits) ? b = "munderover" : b = "msubsup"
+                            v && v.type === "op" && v.limits && t.style === G.DISPLAY || v && v.type === "operatorname" && v.alwaysHandleSupSub && (t.style === G.DISPLAY || v.limits) ? b = "munderover" : b = "msubsup"
                         } else {
                             let v = n.base;
-                            v && v.type === "op" && v.limits && (t.style === $.DISPLAY || v.alwaysHandleSupSub) || v && v.type === "operatorname" && v.alwaysHandleSupSub && (v.limits || t.style === $.DISPLAY) ? b = "munder" : b = "msub"
+                            v && v.type === "op" && v.limits && (t.style === G.DISPLAY || v.alwaysHandleSupSub) || v && v.type === "operatorname" && v.alwaysHandleSupSub && (v.limits || t.style === G.DISPLAY) ? b = "munder" : b = "msub"
                         }
                     else {
                         let v = n.base;
-                        v && v.type === "op" && v.limits && (t.style === $.DISPLAY || v.alwaysHandleSupSub) || v && v.type === "operatorname" && v.alwaysHandleSupSub && (v.limits || t.style === $.DISPLAY) ? b = "mover" : b = "msup"
+                        v && v.type === "op" && v.limits && (t.style === G.DISPLAY || v.alwaysHandleSupSub) || v && v.type === "operatorname" && v.alwaysHandleSupSub && (v.limits || t.style === G.DISPLAY) ? b = "mover" : b = "msup"
                     }
-                    return new V.MathNode(b, f)
+                    return new V.MathNode(b, p)
                 }
-            }), Jt({
+            }), Kt({
                 type: "atom",
                 htmlBuilder(n, t) {
                     return B.mathsym(n.text, n.mode, t, ["m" + n.family])
                 },
                 mathmlBuilder(n, t) {
                     let o = new V.MathNode("mo", [dt(n.text, n.mode)]);
                     if (n.family === "bin") {
-                        let s = tn(n, t);
+                        let s = rn(n, t);
                         s === "bold-italic" && o.setAttribute("mathvariant", s)
                     } else n.family === "punct" ? o.setAttribute("separator", "true") : (n.family === "open" || n.family === "close") && o.setAttribute("stretchy", "false");
                     return o
                 }
             });
-            let Fo = {
+            let Po = {
                 mi: "italic",
                 mn: "normal",
                 mtext: "normal"
             };
-            Jt({
+            Kt({
                 type: "mathord",
                 htmlBuilder(n, t) {
                     return B.makeOrd(n, t, "mathord")
                 },
                 mathmlBuilder(n, t) {
                     let o = new V.MathNode("mi", [dt(n.text, n.mode, t)]),
-                        s = tn(n, t) || "italic";
-                    return s !== Fo[o.type] && o.setAttribute("mathvariant", s), o
+                        s = rn(n, t) || "italic";
+                    return s !== Po[o.type] && o.setAttribute("mathvariant", s), o
                 }
-            }), Jt({
+            }), Kt({
                 type: "textord",
                 htmlBuilder(n, t) {
                     return B.makeOrd(n, t, "textord")
                 },
                 mathmlBuilder(n, t) {
                     let o = dt(n.text, n.mode, t),
-                        s = tn(n, t) || "normal",
+                        s = rn(n, t) || "normal",
                         u;
-                    return n.mode === "text" ? u = new V.MathNode("mtext", [o]) : /[0-9]/.test(n.text) ? u = new V.MathNode("mn", [o]) : n.text === "\\prime" ? u = new V.MathNode("mo", [o]) : u = new V.MathNode("mi", [o]), s !== Fo[u.type] && u.setAttribute("mathvariant", s), u
+                    return n.mode === "text" ? u = new V.MathNode("mtext", [o]) : /[0-9]/.test(n.text) ? u = new V.MathNode("mn", [o]) : n.text === "\\prime" ? u = new V.MathNode("mo", [o]) : u = new V.MathNode("mi", [o]), s !== Po[u.type] && u.setAttribute("mathvariant", s), u
                 }
             });
-            let vn = {
+            let wn = {
                     "\\nobreak": "nobreak",
                     "\\allowbreak": "allowbreak"
                 },
-                wn = {
+                kn = {
                     " ": {},
                     "\\ ": {},
                     "~": {
                         className: "nobreak"
                     },
                     "\\space": {},
                     "\\nobreakspace": {
                         className: "nobreak"
                     }
                 };
-            Jt({
+            Kt({
                 type: "spacing",
                 htmlBuilder(n, t) {
-                    if (wn.hasOwnProperty(n.text)) {
-                        let o = wn[n.text].className || "";
+                    if (kn.hasOwnProperty(n.text)) {
+                        let o = kn[n.text].className || "";
                         if (n.mode === "text") {
                             let s = B.makeOrd(n, t, "textord");
                             return s.classes.push(o), s
                         } else return B.makeSpan(["mspace", o], [B.mathsym(n.text, n.mode, t)], t)
                     } else {
-                        if (vn.hasOwnProperty(n.text)) return B.makeSpan(["mspace", vn[n.text]], [], t);
+                        if (wn.hasOwnProperty(n.text)) return B.makeSpan(["mspace", wn[n.text]], [], t);
                         throw new a('Unknown type of space "' + n.text + '"')
                     }
                 },
                 mathmlBuilder(n, t) {
                     let o;
-                    if (wn.hasOwnProperty(n.text)) o = new V.MathNode("mtext", [new V.TextNode("\xA0")]);
+                    if (kn.hasOwnProperty(n.text)) o = new V.MathNode("mtext", [new V.TextNode("\xA0")]);
                     else {
-                        if (vn.hasOwnProperty(n.text)) return new V.MathNode("mspace");
+                        if (wn.hasOwnProperty(n.text)) return new V.MathNode("mspace");
                         throw new a('Unknown type of space "' + n.text + '"')
                     }
                     return o
                 }
             });
-            let Bo = () => {
+            let Io = () => {
                 let n = new V.MathNode("mtd", []);
                 return n.setAttribute("width", "50%"), n
             };
-            Jt({
+            Kt({
                 type: "tag",
                 mathmlBuilder(n, t) {
-                    let o = new V.MathNode("mtable", [new V.MathNode("mtr", [Bo(), new V.MathNode("mtd", [Ht(n.body, t)]), Bo(), new V.MathNode("mtd", [Ht(n.tag, t)])])]);
+                    let o = new V.MathNode("mtable", [new V.MathNode("mtr", [Io(), new V.MathNode("mtd", [Ht(n.body, t)]), Io(), new V.MathNode("mtd", [Ht(n.tag, t)])])]);
                     return o.setAttribute("width", "100%"), o
                 }
             });
-            let No = {
+            let Oo = {
                     "\\text": void 0,
                     "\\textrm": "textrm",
                     "\\textsf": "textsf",
                     "\\texttt": "texttt",
                     "\\textnormal": "textrm"
                 },
-                Lo = {
+                Ho = {
                     "\\textbf": "textbf",
                     "\\textmd": "textmd"
                 },
-                I1 = {
+                O1 = {
                     "\\textit": "textit",
                     "\\textup": "textup"
                 },
-                Po = (n, t) => {
+                $o = (n, t) => {
                     let o = n.font;
-                    return o ? No[o] ? t.withTextFontFamily(No[o]) : Lo[o] ? t.withTextFontWeight(Lo[o]) : t.withTextFontShape(I1[o]) : t
+                    return o ? Oo[o] ? t.withTextFontFamily(Oo[o]) : Ho[o] ? t.withTextFontWeight(Ho[o]) : t.withTextFontShape(O1[o]) : t
                 };
-            Z({
+            Q({
                 type: "text",
                 names: ["\\text", "\\textrm", "\\textsf", "\\texttt", "\\textnormal", "\\textbf", "\\textmd", "\\textit", "\\textup"],
                 props: {
                     numArgs: 1,
                     argTypes: ["text"],
                     allowedInArgument: !0,
                     allowedInText: !0
@@ -14193,23 +14193,23 @@
                         type: "text",
                         mode: o.mode,
                         body: je(u),
                         font: s
                     }
                 },
                 htmlBuilder(n, t) {
-                    let o = Po(n, t),
-                        s = Qe(n.body, o, !0);
+                    let o = $o(n, t),
+                        s = Ze(n.body, o, !0);
                     return B.makeSpan(["mord", "text"], s, o)
                 },
                 mathmlBuilder(n, t) {
-                    let o = Po(n, t);
+                    let o = $o(n, t);
                     return Ht(n.body, o)
                 }
-            }), Z({
+            }), Q({
                 type: "underline",
                 names: ["\\underline"],
                 props: {
                     numArgs: 1,
                     allowedInText: !0
                 },
                 handler(n, t) {
@@ -14222,15 +14222,15 @@
                         body: t[0]
                     }
                 },
                 htmlBuilder(n, t) {
                     let o = ve(n.body, t),
                         s = B.makeLineSpan("underline-line", t),
                         u = t.fontMetrics().defaultRuleThickness,
-                        f = B.makeVList({
+                        p = B.makeVList({
                             positionType: "top",
                             positionData: o.height,
                             children: [{
                                 type: "kern",
                                 size: u
                             }, {
                                 type: "elem",
@@ -14239,23 +14239,23 @@
                                 type: "kern",
                                 size: 3 * u
                             }, {
                                 type: "elem",
                                 elem: o
                             }]
                         }, t);
-                    return B.makeSpan(["mord", "underline"], [f], t)
+                    return B.makeSpan(["mord", "underline"], [p], t)
                 },
                 mathmlBuilder(n, t) {
                     let o = new V.MathNode("mo", [new V.TextNode("\u203E")]);
                     o.setAttribute("stretchy", "true");
                     let s = new V.MathNode("munder", [Ee(n.body, t), o]);
                     return s.setAttribute("accentunder", "true"), s
                 }
-            }), Z({
+            }), Q({
                 type: "vcenter",
                 names: ["\\vcenter"],
                 props: {
                     numArgs: 1,
                     argTypes: ["original"],
                     allowedInText: !1
                 },
@@ -14281,56 +14281,56 @@
                             elem: o
                         }]
                     }, t)
                 },
                 mathmlBuilder(n, t) {
                     return new V.MathNode("mpadded", [Ee(n.body, t)], ["vcenter"])
                 }
-            }), Z({
+            }), Q({
                 type: "verb",
                 names: ["\\verb"],
                 props: {
                     numArgs: 0,
                     allowedInText: !0
                 },
                 handler(n, t, o) {
                     throw new a("\\verb ended by end of line instead of matching delimiter")
                 },
                 htmlBuilder(n, t) {
-                    let o = Io(n),
+                    let o = Go(n),
                         s = [],
                         u = t.havingStyle(t.style.text());
-                    for (let f = 0; f < o.length; f++) {
-                        let b = o[f];
+                    for (let p = 0; p < o.length; p++) {
+                        let b = o[p];
                         b === "~" && (b = "\\textasciitilde"), s.push(B.makeSymbol(b, "Typewriter-Regular", n.mode, u, ["mord", "texttt"]))
                     }
                     return B.makeSpan(["mord", "text"].concat(u.sizingClasses(t)), B.tryCombineChars(s), u)
                 },
                 mathmlBuilder(n, t) {
-                    let o = new V.TextNode(Io(n)),
+                    let o = new V.TextNode(Go(n)),
                         s = new V.MathNode("mtext", [o]);
                     return s.setAttribute("mathvariant", "monospace"), s
                 }
             });
-            let Io = n => n.body.replace(/ /g, n.star ? "\u2423" : "\xA0");
-            var Gt = Gi;
-            let Oo = `[ \r
+            let Go = n => n.body.replace(/ /g, n.star ? "\u2423" : "\xA0");
+            var Gt = Wi;
+            let Vo = `[ \r
 	]`,
-                O1 = "\\\\[a-zA-Z@]+",
-                H1 = "\\\\[^\uD800-\uDFFF]",
-                $1 = "(" + O1 + ")" + Oo + "*",
-                G1 = `\\\\(
+                H1 = "\\\\[a-zA-Z@]+",
+                $1 = "\\\\[^\uD800-\uDFFF]",
+                G1 = "(" + H1 + ")" + Vo + "*",
+                V1 = `\\\\(
 |[ \r	]+
 ?)[ \r	]*`,
-                kn = "[\u0300-\u036F]",
-                V1 = new RegExp(kn + "+$"),
-                j1 = "(" + Oo + "+)|" + (G1 + "|") + "([!-\\[\\]-\u2027\u202A-\uD7FF\uF900-\uFFFF]" + (kn + "*") + "|[\uD800-\uDBFF][\uDC00-\uDFFF]" + (kn + "*") + "|\\\\verb\\*([^]).*?\\4|\\\\verb([^*a-zA-Z]).*?\\5" + ("|" + $1) + ("|" + H1 + ")");
-            class Ho {
+                _n = "[\u0300-\u036F]",
+                j1 = new RegExp(_n + "+$"),
+                U1 = "(" + Vo + "+)|" + (V1 + "|") + "([!-\\[\\]-\u2027\u202A-\uD7FF\uF900-\uFFFF]" + (_n + "*") + "|[\uD800-\uDBFF][\uDC00-\uDFFF]" + (_n + "*") + "|\\\\verb\\*([^]).*?\\4|\\\\verb([^*a-zA-Z]).*?\\5" + ("|" + G1) + ("|" + $1 + ")");
+            class jo {
                 constructor(t, o) {
-                    this.input = void 0, this.settings = void 0, this.tokenRegex = void 0, this.catcodes = void 0, this.input = t, this.settings = o, this.tokenRegex = new RegExp(j1, "g"), this.catcodes = {
+                    this.input = void 0, this.settings = void 0, this.tokenRegex = void 0, this.catcodes = void 0, this.input = t, this.settings = o, this.tokenRegex = new RegExp(U1, "g"), this.catcodes = {
                         "%": 14,
                         "~": 13
                     }
                 }
                 setCatcode(t, o) {
                     this.catcodes[t] = o
                 }
@@ -14338,22 +14338,22 @@
                     let t = this.input,
                         o = this.tokenRegex.lastIndex;
                     if (o === t.length) return new mt("EOF", new st(this, o, o));
                     let s = this.tokenRegex.exec(t);
                     if (s === null || s.index !== o) throw new a("Unexpected character: '" + t[o] + "'", new mt(t[o], new st(this, o, o + 1)));
                     let u = s[6] || s[3] || (s[2] ? "\\ " : " ");
                     if (this.catcodes[u] === 14) {
-                        let f = t.indexOf(`
+                        let p = t.indexOf(`
 `, this.tokenRegex.lastIndex);
-                        return f === -1 ? (this.tokenRegex.lastIndex = t.length, this.settings.reportNonstrict("commentAtEnd", "% comment has no terminating newline; LaTeX would fail because of commenting the end of math mode (e.g. $)")) : this.tokenRegex.lastIndex = f + 1, this.lex()
+                        return p === -1 ? (this.tokenRegex.lastIndex = t.length, this.settings.reportNonstrict("commentAtEnd", "% comment has no terminating newline; LaTeX would fail because of commenting the end of math mode (e.g. $)")) : this.tokenRegex.lastIndex = p + 1, this.lex()
                     }
                     return new mt(u, new st(this, o, this.tokenRegex.lastIndex))
                 }
             }
-            class U1 {
+            class W1 {
                 constructor(t, o) {
                     t === void 0 && (t = {}), o === void 0 && (o = {}), this.current = void 0, this.builtins = void 0, this.undefStack = void 0, this.current = o, this.builtins = t, this.undefStack = []
                 }
                 beginGroup() {
                     this.undefStack.push({})
                 }
                 endGroup() {
@@ -14377,59 +14377,59 @@
                     } else {
                         let u = this.undefStack[this.undefStack.length - 1];
                         u && !u.hasOwnProperty(t) && (u[t] = this.current[t])
                     }
                     o == null ? delete this.current[t] : this.current[t] = o
                 }
             }
-            var W1 = go;
-            w("\\noexpand", function(n) {
+            var Y1 = vo;
+            k("\\noexpand", function(n) {
                 let t = n.popToken();
                 return n.isExpandable(t.text) && (t.noexpand = !0, t.treatAsRelax = !0), {
                     tokens: [t],
                     numArgs: 0
                 }
-            }), w("\\expandafter", function(n) {
+            }), k("\\expandafter", function(n) {
                 let t = n.popToken();
                 return n.expandOnce(!0), {
                     tokens: [t],
                     numArgs: 0
                 }
-            }), w("\\@firstoftwo", function(n) {
+            }), k("\\@firstoftwo", function(n) {
                 return {
                     tokens: n.consumeArgs(2)[0],
                     numArgs: 0
                 }
-            }), w("\\@secondoftwo", function(n) {
+            }), k("\\@secondoftwo", function(n) {
                 return {
                     tokens: n.consumeArgs(2)[1],
                     numArgs: 0
                 }
-            }), w("\\@ifnextchar", function(n) {
+            }), k("\\@ifnextchar", function(n) {
                 let t = n.consumeArgs(3);
                 n.consumeSpaces();
                 let o = n.future();
                 return t[0].length === 1 && t[0][0].text === o.text ? {
                     tokens: t[1],
                     numArgs: 0
                 } : {
                     tokens: t[2],
                     numArgs: 0
                 }
-            }), w("\\@ifstar", "\\@ifnextchar *{\\@firstoftwo{#1}}"), w("\\TextOrMath", function(n) {
+            }), k("\\@ifstar", "\\@ifnextchar *{\\@firstoftwo{#1}}"), k("\\TextOrMath", function(n) {
                 let t = n.consumeArgs(2);
                 return n.mode === "text" ? {
                     tokens: t[0],
                     numArgs: 0
                 } : {
                     tokens: t[1],
                     numArgs: 0
                 }
             });
-            let $o = {
+            let Uo = {
                 0: 0,
                 1: 1,
                 2: 2,
                 3: 3,
                 4: 4,
                 5: 5,
                 6: 6,
@@ -14445,66 +14445,66 @@
                 d: 13,
                 D: 13,
                 e: 14,
                 E: 14,
                 f: 15,
                 F: 15
             };
-            w("\\char", function(n) {
+            k("\\char", function(n) {
                 let t = n.popToken(),
                     o, s = "";
                 if (t.text === "'") o = 8, t = n.popToken();
                 else if (t.text === '"') o = 16, t = n.popToken();
                 else if (t.text === "`")
                     if (t = n.popToken(), t.text[0] === "\\") s = t.text.charCodeAt(1);
                     else {
                         if (t.text === "EOF") throw new a("\\char` missing argument");
                         s = t.text.charCodeAt(0)
                     }
                 else o = 10;
                 if (o) {
-                    if (s = $o[t.text], s == null || s >= o) throw new a("Invalid base-" + o + " digit " + t.text);
+                    if (s = Uo[t.text], s == null || s >= o) throw new a("Invalid base-" + o + " digit " + t.text);
                     let u;
                     for (;
-                        (u = $o[n.future().text]) != null && u < o;) s *= o, s += u, n.popToken()
+                        (u = Uo[n.future().text]) != null && u < o;) s *= o, s += u, n.popToken()
                 }
                 return "\\@char{" + s + "}"
             });
-            let _n = (n, t, o) => {
+            let Sn = (n, t, o) => {
                 let s = n.consumeArg().tokens;
                 if (s.length !== 1) throw new a("\\newcommand's first argument must be a macro name");
                 let u = s[0].text,
-                    f = n.isDefined(u);
-                if (f && !t) throw new a("\\newcommand{" + u + "} attempting to redefine " + (u + "; use \\renewcommand"));
-                if (!f && !o) throw new a("\\renewcommand{" + u + "} when command " + u + " does not yet exist; use \\newcommand");
+                    p = n.isDefined(u);
+                if (p && !t) throw new a("\\newcommand{" + u + "} attempting to redefine " + (u + "; use \\renewcommand"));
+                if (!p && !o) throw new a("\\renewcommand{" + u + "} when command " + u + " does not yet exist; use \\newcommand");
                 let b = 0;
                 if (s = n.consumeArg().tokens, s.length === 1 && s[0].text === "[") {
                     let v = "",
                         S = n.expandNextToken();
                     for (; S.text !== "]" && S.text !== "EOF";) v += S.text, S = n.expandNextToken();
                     if (!v.match(/^\s*[0-9]+\s*$/)) throw new a("Invalid number of arguments: " + v);
                     b = parseInt(v), s = n.consumeArg().tokens
                 }
                 return n.macros.set(u, {
                     tokens: s,
                     numArgs: b
                 }), ""
             };
-            w("\\newcommand", n => _n(n, !1, !0)), w("\\renewcommand", n => _n(n, !0, !1)), w("\\providecommand", n => _n(n, !0, !0)), w("\\message", n => {
+            k("\\newcommand", n => Sn(n, !1, !0)), k("\\renewcommand", n => Sn(n, !0, !1)), k("\\providecommand", n => Sn(n, !0, !0)), k("\\message", n => {
                 let t = n.consumeArgs(1)[0];
                 return console.log(t.reverse().map(o => o.text).join("")), ""
-            }), w("\\errmessage", n => {
+            }), k("\\errmessage", n => {
                 let t = n.consumeArgs(1)[0];
                 return console.error(t.reverse().map(o => o.text).join("")), ""
-            }), w("\\show", n => {
+            }), k("\\show", n => {
                 let t = n.popToken(),
                     o = t.text;
                 return console.log(t, n.macros.get(o), Gt[o], Oe.math[o], Oe.text[o]), ""
-            }), w("\\bgroup", "{"), w("\\egroup", "}"), w("~", "\\nobreakspace"), w("\\lq", "`"), w("\\rq", "'"), w("\\aa", "\\r a"), w("\\AA", "\\r A"), w("\\textcopyright", "\\html@mathml{\\textcircled{c}}{\\char`\xA9}"), w("\\copyright", "\\TextOrMath{\\textcopyright}{\\text{\\textcopyright}}"), w("\\textregistered", "\\html@mathml{\\textcircled{\\scriptsize R}}{\\char`\xAE}"), w("\u212C", "\\mathscr{B}"), w("\u2130", "\\mathscr{E}"), w("\u2131", "\\mathscr{F}"), w("\u210B", "\\mathscr{H}"), w("\u2110", "\\mathscr{I}"), w("\u2112", "\\mathscr{L}"), w("\u2133", "\\mathscr{M}"), w("\u211B", "\\mathscr{R}"), w("\u212D", "\\mathfrak{C}"), w("\u210C", "\\mathfrak{H}"), w("\u2128", "\\mathfrak{Z}"), w("\\Bbbk", "\\Bbb{k}"), w("\xB7", "\\cdotp"), w("\\llap", "\\mathllap{\\textrm{#1}}"), w("\\rlap", "\\mathrlap{\\textrm{#1}}"), w("\\clap", "\\mathclap{\\textrm{#1}}"), w("\\mathstrut", "\\vphantom{(}"), w("\\underbar", "\\underline{\\text{#1}}"), w("\\not", '\\html@mathml{\\mathrel{\\mathrlap\\@not}}{\\char"338}'), w("\\neq", "\\html@mathml{\\mathrel{\\not=}}{\\mathrel{\\char`\u2260}}"), w("\\ne", "\\neq"), w("\u2260", "\\neq"), w("\\notin", "\\html@mathml{\\mathrel{{\\in}\\mathllap{/\\mskip1mu}}}{\\mathrel{\\char`\u2209}}"), w("\u2209", "\\notin"), w("\u2258", "\\html@mathml{\\mathrel{=\\kern{-1em}\\raisebox{0.4em}{$\\scriptsize\\frown$}}}{\\mathrel{\\char`\u2258}}"), w("\u2259", "\\html@mathml{\\stackrel{\\tiny\\wedge}{=}}{\\mathrel{\\char`\u2258}}"), w("\u225A", "\\html@mathml{\\stackrel{\\tiny\\vee}{=}}{\\mathrel{\\char`\u225A}}"), w("\u225B", "\\html@mathml{\\stackrel{\\scriptsize\\star}{=}}{\\mathrel{\\char`\u225B}}"), w("\u225D", "\\html@mathml{\\stackrel{\\tiny\\mathrm{def}}{=}}{\\mathrel{\\char`\u225D}}"), w("\u225E", "\\html@mathml{\\stackrel{\\tiny\\mathrm{m}}{=}}{\\mathrel{\\char`\u225E}}"), w("\u225F", "\\html@mathml{\\stackrel{\\tiny?}{=}}{\\mathrel{\\char`\u225F}}"), w("\u27C2", "\\perp"), w("\u203C", "\\mathclose{!\\mkern-0.8mu!}"), w("\u220C", "\\notni"), w("\u231C", "\\ulcorner"), w("\u231D", "\\urcorner"), w("\u231E", "\\llcorner"), w("\u231F", "\\lrcorner"), w("\xA9", "\\copyright"), w("\xAE", "\\textregistered"), w("\uFE0F", "\\textregistered"), w("\\ulcorner", '\\html@mathml{\\@ulcorner}{\\mathop{\\char"231c}}'), w("\\urcorner", '\\html@mathml{\\@urcorner}{\\mathop{\\char"231d}}'), w("\\llcorner", '\\html@mathml{\\@llcorner}{\\mathop{\\char"231e}}'), w("\\lrcorner", '\\html@mathml{\\@lrcorner}{\\mathop{\\char"231f}}'), w("\\vdots", "\\mathord{\\varvdots\\rule{0pt}{15pt}}"), w("\u22EE", "\\vdots"), w("\\varGamma", "\\mathit{\\Gamma}"), w("\\varDelta", "\\mathit{\\Delta}"), w("\\varTheta", "\\mathit{\\Theta}"), w("\\varLambda", "\\mathit{\\Lambda}"), w("\\varXi", "\\mathit{\\Xi}"), w("\\varPi", "\\mathit{\\Pi}"), w("\\varSigma", "\\mathit{\\Sigma}"), w("\\varUpsilon", "\\mathit{\\Upsilon}"), w("\\varPhi", "\\mathit{\\Phi}"), w("\\varPsi", "\\mathit{\\Psi}"), w("\\varOmega", "\\mathit{\\Omega}"), w("\\substack", "\\begin{subarray}{c}#1\\end{subarray}"), w("\\colon", "\\nobreak\\mskip2mu\\mathpunct{}\\mathchoice{\\mkern-3mu}{\\mkern-3mu}{}{}{:}\\mskip6mu\\relax"), w("\\boxed", "\\fbox{$\\displaystyle{#1}$}"), w("\\iff", "\\DOTSB\\;\\Longleftrightarrow\\;"), w("\\implies", "\\DOTSB\\;\\Longrightarrow\\;"), w("\\impliedby", "\\DOTSB\\;\\Longleftarrow\\;");
-            let Go = {
+            }), k("\\bgroup", "{"), k("\\egroup", "}"), k("~", "\\nobreakspace"), k("\\lq", "`"), k("\\rq", "'"), k("\\aa", "\\r a"), k("\\AA", "\\r A"), k("\\textcopyright", "\\html@mathml{\\textcircled{c}}{\\char`\xA9}"), k("\\copyright", "\\TextOrMath{\\textcopyright}{\\text{\\textcopyright}}"), k("\\textregistered", "\\html@mathml{\\textcircled{\\scriptsize R}}{\\char`\xAE}"), k("\u212C", "\\mathscr{B}"), k("\u2130", "\\mathscr{E}"), k("\u2131", "\\mathscr{F}"), k("\u210B", "\\mathscr{H}"), k("\u2110", "\\mathscr{I}"), k("\u2112", "\\mathscr{L}"), k("\u2133", "\\mathscr{M}"), k("\u211B", "\\mathscr{R}"), k("\u212D", "\\mathfrak{C}"), k("\u210C", "\\mathfrak{H}"), k("\u2128", "\\mathfrak{Z}"), k("\\Bbbk", "\\Bbb{k}"), k("\xB7", "\\cdotp"), k("\\llap", "\\mathllap{\\textrm{#1}}"), k("\\rlap", "\\mathrlap{\\textrm{#1}}"), k("\\clap", "\\mathclap{\\textrm{#1}}"), k("\\mathstrut", "\\vphantom{(}"), k("\\underbar", "\\underline{\\text{#1}}"), k("\\not", '\\html@mathml{\\mathrel{\\mathrlap\\@not}}{\\char"338}'), k("\\neq", "\\html@mathml{\\mathrel{\\not=}}{\\mathrel{\\char`\u2260}}"), k("\\ne", "\\neq"), k("\u2260", "\\neq"), k("\\notin", "\\html@mathml{\\mathrel{{\\in}\\mathllap{/\\mskip1mu}}}{\\mathrel{\\char`\u2209}}"), k("\u2209", "\\notin"), k("\u2258", "\\html@mathml{\\mathrel{=\\kern{-1em}\\raisebox{0.4em}{$\\scriptsize\\frown$}}}{\\mathrel{\\char`\u2258}}"), k("\u2259", "\\html@mathml{\\stackrel{\\tiny\\wedge}{=}}{\\mathrel{\\char`\u2258}}"), k("\u225A", "\\html@mathml{\\stackrel{\\tiny\\vee}{=}}{\\mathrel{\\char`\u225A}}"), k("\u225B", "\\html@mathml{\\stackrel{\\scriptsize\\star}{=}}{\\mathrel{\\char`\u225B}}"), k("\u225D", "\\html@mathml{\\stackrel{\\tiny\\mathrm{def}}{=}}{\\mathrel{\\char`\u225D}}"), k("\u225E", "\\html@mathml{\\stackrel{\\tiny\\mathrm{m}}{=}}{\\mathrel{\\char`\u225E}}"), k("\u225F", "\\html@mathml{\\stackrel{\\tiny?}{=}}{\\mathrel{\\char`\u225F}}"), k("\u27C2", "\\perp"), k("\u203C", "\\mathclose{!\\mkern-0.8mu!}"), k("\u220C", "\\notni"), k("\u231C", "\\ulcorner"), k("\u231D", "\\urcorner"), k("\u231E", "\\llcorner"), k("\u231F", "\\lrcorner"), k("\xA9", "\\copyright"), k("\xAE", "\\textregistered"), k("\uFE0F", "\\textregistered"), k("\\ulcorner", '\\html@mathml{\\@ulcorner}{\\mathop{\\char"231c}}'), k("\\urcorner", '\\html@mathml{\\@urcorner}{\\mathop{\\char"231d}}'), k("\\llcorner", '\\html@mathml{\\@llcorner}{\\mathop{\\char"231e}}'), k("\\lrcorner", '\\html@mathml{\\@lrcorner}{\\mathop{\\char"231f}}'), k("\\vdots", "\\mathord{\\varvdots\\rule{0pt}{15pt}}"), k("\u22EE", "\\vdots"), k("\\varGamma", "\\mathit{\\Gamma}"), k("\\varDelta", "\\mathit{\\Delta}"), k("\\varTheta", "\\mathit{\\Theta}"), k("\\varLambda", "\\mathit{\\Lambda}"), k("\\varXi", "\\mathit{\\Xi}"), k("\\varPi", "\\mathit{\\Pi}"), k("\\varSigma", "\\mathit{\\Sigma}"), k("\\varUpsilon", "\\mathit{\\Upsilon}"), k("\\varPhi", "\\mathit{\\Phi}"), k("\\varPsi", "\\mathit{\\Psi}"), k("\\varOmega", "\\mathit{\\Omega}"), k("\\substack", "\\begin{subarray}{c}#1\\end{subarray}"), k("\\colon", "\\nobreak\\mskip2mu\\mathpunct{}\\mathchoice{\\mkern-3mu}{\\mkern-3mu}{}{}{:}\\mskip6mu\\relax"), k("\\boxed", "\\fbox{$\\displaystyle{#1}$}"), k("\\iff", "\\DOTSB\\;\\Longleftrightarrow\\;"), k("\\implies", "\\DOTSB\\;\\Longrightarrow\\;"), k("\\impliedby", "\\DOTSB\\;\\Longleftarrow\\;");
+            let Wo = {
                 ",": "\\dotsc",
                 "\\not": "\\dotsb",
                 "+": "\\dotsb",
                 "=": "\\dotsb",
                 "<": "\\dotsb",
                 ">": "\\dotsb",
                 "-": "\\dotsb",
@@ -14545,20 +14545,20 @@
                 "\\oint": "\\dotsi",
                 "\\iint": "\\dotsi",
                 "\\iiint": "\\dotsi",
                 "\\iiiint": "\\dotsi",
                 "\\idotsint": "\\dotsi",
                 "\\DOTSX": "\\dotsx"
             };
-            w("\\dots", function(n) {
+            k("\\dots", function(n) {
                 let t = "\\dotso",
                     o = n.expandAfterFuture().text;
-                return o in Go ? t = Go[o] : (o.slice(0, 4) === "\\not" || o in Oe.math && R.contains(["bin", "rel"], Oe.math[o].group)) && (t = "\\dotsb"), t
+                return o in Wo ? t = Wo[o] : (o.slice(0, 4) === "\\not" || o in Oe.math && R.contains(["bin", "rel"], Oe.math[o].group)) && (t = "\\dotsb"), t
             });
-            let Sn = {
+            let Cn = {
                 ")": !0,
                 "]": !0,
                 "\\rbrack": !0,
                 "\\}": !0,
                 "\\rbrace": !0,
                 "\\rangle": !0,
                 "\\rceil": !0,
@@ -14571,64 +14571,64 @@
                 "\\Bigr": !0,
                 "\\Biggr": !0,
                 $: !0,
                 ";": !0,
                 ".": !0,
                 ",": !0
             };
-            w("\\dotso", function(n) {
-                return n.future().text in Sn ? "\\ldots\\," : "\\ldots"
-            }), w("\\dotsc", function(n) {
+            k("\\dotso", function(n) {
+                return n.future().text in Cn ? "\\ldots\\," : "\\ldots"
+            }), k("\\dotsc", function(n) {
                 let t = n.future().text;
-                return t in Sn && t !== "," ? "\\ldots\\," : "\\ldots"
-            }), w("\\cdots", function(n) {
-                return n.future().text in Sn ? "\\@cdots\\," : "\\@cdots"
-            }), w("\\dotsb", "\\cdots"), w("\\dotsm", "\\cdots"), w("\\dotsi", "\\!\\cdots"), w("\\dotsx", "\\ldots\\,"), w("\\DOTSI", "\\relax"), w("\\DOTSB", "\\relax"), w("\\DOTSX", "\\relax"), w("\\tmspace", "\\TextOrMath{\\kern#1#3}{\\mskip#1#2}\\relax"), w("\\,", "\\tmspace+{3mu}{.1667em}"), w("\\thinspace", "\\,"), w("\\>", "\\mskip{4mu}"), w("\\:", "\\tmspace+{4mu}{.2222em}"), w("\\medspace", "\\:"), w("\\;", "\\tmspace+{5mu}{.2777em}"), w("\\thickspace", "\\;"), w("\\!", "\\tmspace-{3mu}{.1667em}"), w("\\negthinspace", "\\!"), w("\\negmedspace", "\\tmspace-{4mu}{.2222em}"), w("\\negthickspace", "\\tmspace-{5mu}{.277em}"), w("\\enspace", "\\kern.5em "), w("\\enskip", "\\hskip.5em\\relax"), w("\\quad", "\\hskip1em\\relax"), w("\\qquad", "\\hskip2em\\relax"), w("\\tag", "\\@ifstar\\tag@literal\\tag@paren"), w("\\tag@paren", "\\tag@literal{({#1})}"), w("\\tag@literal", n => {
+                return t in Cn && t !== "," ? "\\ldots\\," : "\\ldots"
+            }), k("\\cdots", function(n) {
+                return n.future().text in Cn ? "\\@cdots\\," : "\\@cdots"
+            }), k("\\dotsb", "\\cdots"), k("\\dotsm", "\\cdots"), k("\\dotsi", "\\!\\cdots"), k("\\dotsx", "\\ldots\\,"), k("\\DOTSI", "\\relax"), k("\\DOTSB", "\\relax"), k("\\DOTSX", "\\relax"), k("\\tmspace", "\\TextOrMath{\\kern#1#3}{\\mskip#1#2}\\relax"), k("\\,", "\\tmspace+{3mu}{.1667em}"), k("\\thinspace", "\\,"), k("\\>", "\\mskip{4mu}"), k("\\:", "\\tmspace+{4mu}{.2222em}"), k("\\medspace", "\\:"), k("\\;", "\\tmspace+{5mu}{.2777em}"), k("\\thickspace", "\\;"), k("\\!", "\\tmspace-{3mu}{.1667em}"), k("\\negthinspace", "\\!"), k("\\negmedspace", "\\tmspace-{4mu}{.2222em}"), k("\\negthickspace", "\\tmspace-{5mu}{.277em}"), k("\\enspace", "\\kern.5em "), k("\\enskip", "\\hskip.5em\\relax"), k("\\quad", "\\hskip1em\\relax"), k("\\qquad", "\\hskip2em\\relax"), k("\\tag", "\\@ifstar\\tag@literal\\tag@paren"), k("\\tag@paren", "\\tag@literal{({#1})}"), k("\\tag@literal", n => {
                 if (n.macros.get("\\df@tag")) throw new a("Multiple \\tag");
                 return "\\gdef\\df@tag{\\text{#1}}"
-            }), w("\\bmod", "\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}\\mathbin{\\rm mod}\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}"), w("\\pod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern8mu}{\\mkern8mu}{\\mkern8mu}(#1)"), w("\\pmod", "\\pod{{\\rm mod}\\mkern6mu#1}"), w("\\mod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern12mu}{\\mkern12mu}{\\mkern12mu}{\\rm mod}\\,\\,#1"), w("\\newline", "\\\\\\relax"), w("\\TeX", "\\textrm{\\html@mathml{T\\kern-.1667em\\raisebox{-.5ex}{E}\\kern-.125emX}{TeX}}");
-            let Vo = Q(vt["Main-Regular"][84][1] - .7 * vt["Main-Regular"][65][1]);
-            w("\\LaTeX", "\\textrm{\\html@mathml{" + ("L\\kern-.36em\\raisebox{" + Vo + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{LaTeX}}"), w("\\KaTeX", "\\textrm{\\html@mathml{" + ("K\\kern-.17em\\raisebox{" + Vo + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{KaTeX}}"), w("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), w("\\@hspace", "\\hskip #1\\relax"), w("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), w("\\ordinarycolon", ":"), w("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), w("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), w("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), w("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), w("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), w("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), w("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), w("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), w("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), w("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), w("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), w("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), w("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), w("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), w("\u2237", "\\dblcolon"), w("\u2239", "\\eqcolon"), w("\u2254", "\\coloneqq"), w("\u2255", "\\eqqcolon"), w("\u2A74", "\\Coloneqq"), w("\\ratio", "\\vcentcolon"), w("\\coloncolon", "\\dblcolon"), w("\\colonequals", "\\coloneqq"), w("\\coloncolonequals", "\\Coloneqq"), w("\\equalscolon", "\\eqqcolon"), w("\\equalscoloncolon", "\\Eqqcolon"), w("\\colonminus", "\\coloneq"), w("\\coloncolonminus", "\\Coloneq"), w("\\minuscolon", "\\eqcolon"), w("\\minuscoloncolon", "\\Eqcolon"), w("\\coloncolonapprox", "\\Colonapprox"), w("\\coloncolonsim", "\\Colonsim"), w("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), w("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), w("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), w("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), w("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`\u220C}}"), w("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), w("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), w("\\injlim", "\\DOTSB\\operatorname*{inj\\,lim}"), w("\\projlim", "\\DOTSB\\operatorname*{proj\\,lim}"), w("\\varlimsup", "\\DOTSB\\operatorname*{\\overline{lim}}"), w("\\varliminf", "\\DOTSB\\operatorname*{\\underline{lim}}"), w("\\varinjlim", "\\DOTSB\\operatorname*{\\underrightarrow{lim}}"), w("\\varprojlim", "\\DOTSB\\operatorname*{\\underleftarrow{lim}}"), w("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{\u2269}"), w("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{\u2268}"), w("\\ngeqq", "\\html@mathml{\\@ngeqq}{\u2271}"), w("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{\u2271}"), w("\\nleqq", "\\html@mathml{\\@nleqq}{\u2270}"), w("\\nleqslant", "\\html@mathml{\\@nleqslant}{\u2270}"), w("\\nshortmid", "\\html@mathml{\\@nshortmid}{\u2224}"), w("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{\u2226}"), w("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{\u2288}"), w("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{\u2289}"), w("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{\u228A}"), w("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{\u2ACB}"), w("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{\u228B}"), w("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{\u2ACC}"), w("\\imath", "\\html@mathml{\\@imath}{\u0131}"), w("\\jmath", "\\html@mathml{\\@jmath}{\u0237}"), w("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`\u27E6}}"), w("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`\u27E7}}"), w("\u27E6", "\\llbracket"), w("\u27E7", "\\rrbracket"), w("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`\u2983}}"), w("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`\u2984}}"), w("\u2983", "\\lBrace"), w("\u2984", "\\rBrace"), w("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`\u29B5}}"), w("\u29B5", "\\minuso"), w("\\darr", "\\downarrow"), w("\\dArr", "\\Downarrow"), w("\\Darr", "\\Downarrow"), w("\\lang", "\\langle"), w("\\rang", "\\rangle"), w("\\uarr", "\\uparrow"), w("\\uArr", "\\Uparrow"), w("\\Uarr", "\\Uparrow"), w("\\N", "\\mathbb{N}"), w("\\R", "\\mathbb{R}"), w("\\Z", "\\mathbb{Z}"), w("\\alef", "\\aleph"), w("\\alefsym", "\\aleph"), w("\\Alpha", "\\mathrm{A}"), w("\\Beta", "\\mathrm{B}"), w("\\bull", "\\bullet"), w("\\Chi", "\\mathrm{X}"), w("\\clubs", "\\clubsuit"), w("\\cnums", "\\mathbb{C}"), w("\\Complex", "\\mathbb{C}"), w("\\Dagger", "\\ddagger"), w("\\diamonds", "\\diamondsuit"), w("\\empty", "\\emptyset"), w("\\Epsilon", "\\mathrm{E}"), w("\\Eta", "\\mathrm{H}"), w("\\exist", "\\exists"), w("\\harr", "\\leftrightarrow"), w("\\hArr", "\\Leftrightarrow"), w("\\Harr", "\\Leftrightarrow"), w("\\hearts", "\\heartsuit"), w("\\image", "\\Im"), w("\\infin", "\\infty"), w("\\Iota", "\\mathrm{I}"), w("\\isin", "\\in"), w("\\Kappa", "\\mathrm{K}"), w("\\larr", "\\leftarrow"), w("\\lArr", "\\Leftarrow"), w("\\Larr", "\\Leftarrow"), w("\\lrarr", "\\leftrightarrow"), w("\\lrArr", "\\Leftrightarrow"), w("\\Lrarr", "\\Leftrightarrow"), w("\\Mu", "\\mathrm{M}"), w("\\natnums", "\\mathbb{N}"), w("\\Nu", "\\mathrm{N}"), w("\\Omicron", "\\mathrm{O}"), w("\\plusmn", "\\pm"), w("\\rarr", "\\rightarrow"), w("\\rArr", "\\Rightarrow"), w("\\Rarr", "\\Rightarrow"), w("\\real", "\\Re"), w("\\reals", "\\mathbb{R}"), w("\\Reals", "\\mathbb{R}"), w("\\Rho", "\\mathrm{P}"), w("\\sdot", "\\cdot"), w("\\sect", "\\S"), w("\\spades", "\\spadesuit"), w("\\sub", "\\subset"), w("\\sube", "\\subseteq"), w("\\supe", "\\supseteq"), w("\\Tau", "\\mathrm{T}"), w("\\thetasym", "\\vartheta"), w("\\weierp", "\\wp"), w("\\Zeta", "\\mathrm{Z}"), w("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), w("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), w("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), w("\\bra", "\\mathinner{\\langle{#1}|}"), w("\\ket", "\\mathinner{|{#1}\\rangle}"), w("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), w("\\Bra", "\\left\\langle#1\\right|"), w("\\Ket", "\\left|#1\\right\\rangle");
-            let jo = n => t => {
+            }), k("\\bmod", "\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}\\mathbin{\\rm mod}\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}"), k("\\pod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern8mu}{\\mkern8mu}{\\mkern8mu}(#1)"), k("\\pmod", "\\pod{{\\rm mod}\\mkern6mu#1}"), k("\\mod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern12mu}{\\mkern12mu}{\\mkern12mu}{\\rm mod}\\,\\,#1"), k("\\newline", "\\\\\\relax"), k("\\TeX", "\\textrm{\\html@mathml{T\\kern-.1667em\\raisebox{-.5ex}{E}\\kern-.125emX}{TeX}}");
+            let Yo = Z(vt["Main-Regular"][84][1] - .7 * vt["Main-Regular"][65][1]);
+            k("\\LaTeX", "\\textrm{\\html@mathml{" + ("L\\kern-.36em\\raisebox{" + Yo + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{LaTeX}}"), k("\\KaTeX", "\\textrm{\\html@mathml{" + ("K\\kern-.17em\\raisebox{" + Yo + "}{\\scriptstyle A}") + "\\kern-.15em\\TeX}{KaTeX}}"), k("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), k("\\@hspace", "\\hskip #1\\relax"), k("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), k("\\ordinarycolon", ":"), k("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), k("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), k("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), k("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), k("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), k("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), k("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), k("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), k("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), k("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), k("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), k("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), k("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), k("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), k("\u2237", "\\dblcolon"), k("\u2239", "\\eqcolon"), k("\u2254", "\\coloneqq"), k("\u2255", "\\eqqcolon"), k("\u2A74", "\\Coloneqq"), k("\\ratio", "\\vcentcolon"), k("\\coloncolon", "\\dblcolon"), k("\\colonequals", "\\coloneqq"), k("\\coloncolonequals", "\\Coloneqq"), k("\\equalscolon", "\\eqqcolon"), k("\\equalscoloncolon", "\\Eqqcolon"), k("\\colonminus", "\\coloneq"), k("\\coloncolonminus", "\\Coloneq"), k("\\minuscolon", "\\eqcolon"), k("\\minuscoloncolon", "\\Eqcolon"), k("\\coloncolonapprox", "\\Colonapprox"), k("\\coloncolonsim", "\\Colonsim"), k("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), k("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), k("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), k("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), k("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`\u220C}}"), k("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), k("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), k("\\injlim", "\\DOTSB\\operatorname*{inj\\,lim}"), k("\\projlim", "\\DOTSB\\operatorname*{proj\\,lim}"), k("\\varlimsup", "\\DOTSB\\operatorname*{\\overline{lim}}"), k("\\varliminf", "\\DOTSB\\operatorname*{\\underline{lim}}"), k("\\varinjlim", "\\DOTSB\\operatorname*{\\underrightarrow{lim}}"), k("\\varprojlim", "\\DOTSB\\operatorname*{\\underleftarrow{lim}}"), k("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{\u2269}"), k("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{\u2268}"), k("\\ngeqq", "\\html@mathml{\\@ngeqq}{\u2271}"), k("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{\u2271}"), k("\\nleqq", "\\html@mathml{\\@nleqq}{\u2270}"), k("\\nleqslant", "\\html@mathml{\\@nleqslant}{\u2270}"), k("\\nshortmid", "\\html@mathml{\\@nshortmid}{\u2224}"), k("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{\u2226}"), k("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{\u2288}"), k("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{\u2289}"), k("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{\u228A}"), k("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{\u2ACB}"), k("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{\u228B}"), k("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{\u2ACC}"), k("\\imath", "\\html@mathml{\\@imath}{\u0131}"), k("\\jmath", "\\html@mathml{\\@jmath}{\u0237}"), k("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`\u27E6}}"), k("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`\u27E7}}"), k("\u27E6", "\\llbracket"), k("\u27E7", "\\rrbracket"), k("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`\u2983}}"), k("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`\u2984}}"), k("\u2983", "\\lBrace"), k("\u2984", "\\rBrace"), k("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`\u29B5}}"), k("\u29B5", "\\minuso"), k("\\darr", "\\downarrow"), k("\\dArr", "\\Downarrow"), k("\\Darr", "\\Downarrow"), k("\\lang", "\\langle"), k("\\rang", "\\rangle"), k("\\uarr", "\\uparrow"), k("\\uArr", "\\Uparrow"), k("\\Uarr", "\\Uparrow"), k("\\N", "\\mathbb{N}"), k("\\R", "\\mathbb{R}"), k("\\Z", "\\mathbb{Z}"), k("\\alef", "\\aleph"), k("\\alefsym", "\\aleph"), k("\\Alpha", "\\mathrm{A}"), k("\\Beta", "\\mathrm{B}"), k("\\bull", "\\bullet"), k("\\Chi", "\\mathrm{X}"), k("\\clubs", "\\clubsuit"), k("\\cnums", "\\mathbb{C}"), k("\\Complex", "\\mathbb{C}"), k("\\Dagger", "\\ddagger"), k("\\diamonds", "\\diamondsuit"), k("\\empty", "\\emptyset"), k("\\Epsilon", "\\mathrm{E}"), k("\\Eta", "\\mathrm{H}"), k("\\exist", "\\exists"), k("\\harr", "\\leftrightarrow"), k("\\hArr", "\\Leftrightarrow"), k("\\Harr", "\\Leftrightarrow"), k("\\hearts", "\\heartsuit"), k("\\image", "\\Im"), k("\\infin", "\\infty"), k("\\Iota", "\\mathrm{I}"), k("\\isin", "\\in"), k("\\Kappa", "\\mathrm{K}"), k("\\larr", "\\leftarrow"), k("\\lArr", "\\Leftarrow"), k("\\Larr", "\\Leftarrow"), k("\\lrarr", "\\leftrightarrow"), k("\\lrArr", "\\Leftrightarrow"), k("\\Lrarr", "\\Leftrightarrow"), k("\\Mu", "\\mathrm{M}"), k("\\natnums", "\\mathbb{N}"), k("\\Nu", "\\mathrm{N}"), k("\\Omicron", "\\mathrm{O}"), k("\\plusmn", "\\pm"), k("\\rarr", "\\rightarrow"), k("\\rArr", "\\Rightarrow"), k("\\Rarr", "\\Rightarrow"), k("\\real", "\\Re"), k("\\reals", "\\mathbb{R}"), k("\\Reals", "\\mathbb{R}"), k("\\Rho", "\\mathrm{P}"), k("\\sdot", "\\cdot"), k("\\sect", "\\S"), k("\\spades", "\\spadesuit"), k("\\sub", "\\subset"), k("\\sube", "\\subseteq"), k("\\supe", "\\supseteq"), k("\\Tau", "\\mathrm{T}"), k("\\thetasym", "\\vartheta"), k("\\weierp", "\\wp"), k("\\Zeta", "\\mathrm{Z}"), k("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), k("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), k("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), k("\\bra", "\\mathinner{\\langle{#1}|}"), k("\\ket", "\\mathinner{|{#1}\\rangle}"), k("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), k("\\Bra", "\\left\\langle#1\\right|"), k("\\Ket", "\\left|#1\\right\\rangle");
+            let Zo = n => t => {
                 let o = t.consumeArg().tokens,
                     s = t.consumeArg().tokens,
                     u = t.consumeArg().tokens,
-                    f = t.consumeArg().tokens,
+                    p = t.consumeArg().tokens,
                     b = t.macros.get("|"),
                     v = t.macros.get("\\|");
                 t.macros.beginGroup();
                 let S = F => N => {
                     n && (N.macros.set("|", b), u.length && N.macros.set("\\|", v));
-                    let O = F;
-                    return !F && u.length && N.future().text === "|" && (N.popToken(), O = !0), {
-                        tokens: O ? u : s,
+                    let H = F;
+                    return !F && u.length && N.future().text === "|" && (N.popToken(), H = !0), {
+                        tokens: H ? u : s,
                         numArgs: 0
                     }
                 };
                 t.macros.set("|", S(!1)), u.length && t.macros.set("\\|", S(!0));
                 let E = t.consumeArg().tokens,
-                    z = t.expandTokens([...f, ...E, ...o]);
+                    z = t.expandTokens([...p, ...E, ...o]);
                 return t.macros.endGroup(), {
                     tokens: z.reverse(),
                     numArgs: 0
                 }
             };
-            w("\\bra@ket", jo(!1)), w("\\bra@set", jo(!0)), w("\\Braket", "\\bra@ket{\\left\\langle}{\\,\\middle\\vert\\,}{\\,\\middle\\vert\\,}{\\right\\rangle}"), w("\\Set", "\\bra@set{\\left\\{\\:}{\\;\\middle\\vert\\;}{\\;\\middle\\Vert\\;}{\\:\\right\\}}"), w("\\set", "\\bra@set{\\{\\,}{\\mid}{}{\\,\\}}"), w("\\angln", "{\\angl n}"), w("\\blue", "\\textcolor{##6495ed}{#1}"), w("\\orange", "\\textcolor{##ffa500}{#1}"), w("\\pink", "\\textcolor{##ff00af}{#1}"), w("\\red", "\\textcolor{##df0030}{#1}"), w("\\green", "\\textcolor{##28ae7b}{#1}"), w("\\gray", "\\textcolor{gray}{#1}"), w("\\purple", "\\textcolor{##9d38bd}{#1}"), w("\\blueA", "\\textcolor{##ccfaff}{#1}"), w("\\blueB", "\\textcolor{##80f6ff}{#1}"), w("\\blueC", "\\textcolor{##63d9ea}{#1}"), w("\\blueD", "\\textcolor{##11accd}{#1}"), w("\\blueE", "\\textcolor{##0c7f99}{#1}"), w("\\tealA", "\\textcolor{##94fff5}{#1}"), w("\\tealB", "\\textcolor{##26edd5}{#1}"), w("\\tealC", "\\textcolor{##01d1c1}{#1}"), w("\\tealD", "\\textcolor{##01a995}{#1}"), w("\\tealE", "\\textcolor{##208170}{#1}"), w("\\greenA", "\\textcolor{##b6ffb0}{#1}"), w("\\greenB", "\\textcolor{##8af281}{#1}"), w("\\greenC", "\\textcolor{##74cf70}{#1}"), w("\\greenD", "\\textcolor{##1fab54}{#1}"), w("\\greenE", "\\textcolor{##0d923f}{#1}"), w("\\goldA", "\\textcolor{##ffd0a9}{#1}"), w("\\goldB", "\\textcolor{##ffbb71}{#1}"), w("\\goldC", "\\textcolor{##ff9c39}{#1}"), w("\\goldD", "\\textcolor{##e07d10}{#1}"), w("\\goldE", "\\textcolor{##a75a05}{#1}"), w("\\redA", "\\textcolor{##fca9a9}{#1}"), w("\\redB", "\\textcolor{##ff8482}{#1}"), w("\\redC", "\\textcolor{##f9685d}{#1}"), w("\\redD", "\\textcolor{##e84d39}{#1}"), w("\\redE", "\\textcolor{##bc2612}{#1}"), w("\\maroonA", "\\textcolor{##ffbde0}{#1}"), w("\\maroonB", "\\textcolor{##ff92c6}{#1}"), w("\\maroonC", "\\textcolor{##ed5fa6}{#1}"), w("\\maroonD", "\\textcolor{##ca337c}{#1}"), w("\\maroonE", "\\textcolor{##9e034e}{#1}"), w("\\purpleA", "\\textcolor{##ddd7ff}{#1}"), w("\\purpleB", "\\textcolor{##c6b9fc}{#1}"), w("\\purpleC", "\\textcolor{##aa87ff}{#1}"), w("\\purpleD", "\\textcolor{##7854ab}{#1}"), w("\\purpleE", "\\textcolor{##543b78}{#1}"), w("\\mintA", "\\textcolor{##f5f9e8}{#1}"), w("\\mintB", "\\textcolor{##edf2df}{#1}"), w("\\mintC", "\\textcolor{##e0e5cc}{#1}"), w("\\grayA", "\\textcolor{##f6f7f7}{#1}"), w("\\grayB", "\\textcolor{##f0f1f2}{#1}"), w("\\grayC", "\\textcolor{##e3e5e6}{#1}"), w("\\grayD", "\\textcolor{##d6d8da}{#1}"), w("\\grayE", "\\textcolor{##babec2}{#1}"), w("\\grayF", "\\textcolor{##888d93}{#1}"), w("\\grayG", "\\textcolor{##626569}{#1}"), w("\\grayH", "\\textcolor{##3b3e40}{#1}"), w("\\grayI", "\\textcolor{##21242c}{#1}"), w("\\kaBlue", "\\textcolor{##314453}{#1}"), w("\\kaGreen", "\\textcolor{##71B307}{#1}");
-            let Uo = {
+            k("\\bra@ket", Zo(!1)), k("\\bra@set", Zo(!0)), k("\\Braket", "\\bra@ket{\\left\\langle}{\\,\\middle\\vert\\,}{\\,\\middle\\vert\\,}{\\right\\rangle}"), k("\\Set", "\\bra@set{\\left\\{\\:}{\\;\\middle\\vert\\;}{\\;\\middle\\Vert\\;}{\\:\\right\\}}"), k("\\set", "\\bra@set{\\{\\,}{\\mid}{}{\\,\\}}"), k("\\angln", "{\\angl n}"), k("\\blue", "\\textcolor{##6495ed}{#1}"), k("\\orange", "\\textcolor{##ffa500}{#1}"), k("\\pink", "\\textcolor{##ff00af}{#1}"), k("\\red", "\\textcolor{##df0030}{#1}"), k("\\green", "\\textcolor{##28ae7b}{#1}"), k("\\gray", "\\textcolor{gray}{#1}"), k("\\purple", "\\textcolor{##9d38bd}{#1}"), k("\\blueA", "\\textcolor{##ccfaff}{#1}"), k("\\blueB", "\\textcolor{##80f6ff}{#1}"), k("\\blueC", "\\textcolor{##63d9ea}{#1}"), k("\\blueD", "\\textcolor{##11accd}{#1}"), k("\\blueE", "\\textcolor{##0c7f99}{#1}"), k("\\tealA", "\\textcolor{##94fff5}{#1}"), k("\\tealB", "\\textcolor{##26edd5}{#1}"), k("\\tealC", "\\textcolor{##01d1c1}{#1}"), k("\\tealD", "\\textcolor{##01a995}{#1}"), k("\\tealE", "\\textcolor{##208170}{#1}"), k("\\greenA", "\\textcolor{##b6ffb0}{#1}"), k("\\greenB", "\\textcolor{##8af281}{#1}"), k("\\greenC", "\\textcolor{##74cf70}{#1}"), k("\\greenD", "\\textcolor{##1fab54}{#1}"), k("\\greenE", "\\textcolor{##0d923f}{#1}"), k("\\goldA", "\\textcolor{##ffd0a9}{#1}"), k("\\goldB", "\\textcolor{##ffbb71}{#1}"), k("\\goldC", "\\textcolor{##ff9c39}{#1}"), k("\\goldD", "\\textcolor{##e07d10}{#1}"), k("\\goldE", "\\textcolor{##a75a05}{#1}"), k("\\redA", "\\textcolor{##fca9a9}{#1}"), k("\\redB", "\\textcolor{##ff8482}{#1}"), k("\\redC", "\\textcolor{##f9685d}{#1}"), k("\\redD", "\\textcolor{##e84d39}{#1}"), k("\\redE", "\\textcolor{##bc2612}{#1}"), k("\\maroonA", "\\textcolor{##ffbde0}{#1}"), k("\\maroonB", "\\textcolor{##ff92c6}{#1}"), k("\\maroonC", "\\textcolor{##ed5fa6}{#1}"), k("\\maroonD", "\\textcolor{##ca337c}{#1}"), k("\\maroonE", "\\textcolor{##9e034e}{#1}"), k("\\purpleA", "\\textcolor{##ddd7ff}{#1}"), k("\\purpleB", "\\textcolor{##c6b9fc}{#1}"), k("\\purpleC", "\\textcolor{##aa87ff}{#1}"), k("\\purpleD", "\\textcolor{##7854ab}{#1}"), k("\\purpleE", "\\textcolor{##543b78}{#1}"), k("\\mintA", "\\textcolor{##f5f9e8}{#1}"), k("\\mintB", "\\textcolor{##edf2df}{#1}"), k("\\mintC", "\\textcolor{##e0e5cc}{#1}"), k("\\grayA", "\\textcolor{##f6f7f7}{#1}"), k("\\grayB", "\\textcolor{##f0f1f2}{#1}"), k("\\grayC", "\\textcolor{##e3e5e6}{#1}"), k("\\grayD", "\\textcolor{##d6d8da}{#1}"), k("\\grayE", "\\textcolor{##babec2}{#1}"), k("\\grayF", "\\textcolor{##888d93}{#1}"), k("\\grayG", "\\textcolor{##626569}{#1}"), k("\\grayH", "\\textcolor{##3b3e40}{#1}"), k("\\grayI", "\\textcolor{##21242c}{#1}"), k("\\kaBlue", "\\textcolor{##314453}{#1}"), k("\\kaGreen", "\\textcolor{##71B307}{#1}");
+            let Qo = {
                 "^": !0,
                 _: !0,
                 "\\limits": !0,
                 "\\nolimits": !0
             };
-            class Y1 {
+            class Z1 {
                 constructor(t, o, s) {
-                    this.settings = void 0, this.expansionCount = void 0, this.lexer = void 0, this.macros = void 0, this.stack = void 0, this.mode = void 0, this.settings = o, this.expansionCount = 0, this.feed(t), this.macros = new U1(W1, o.macros), this.mode = s, this.stack = []
+                    this.settings = void 0, this.expansionCount = void 0, this.lexer = void 0, this.macros = void 0, this.stack = void 0, this.mode = void 0, this.settings = o, this.expansionCount = 0, this.feed(t), this.macros = new W1(Y1, o.macros), this.mode = s, this.stack = []
                 }
                 feed(t) {
-                    this.lexer = new Ho(t, this.settings)
+                    this.lexer = new jo(t, this.settings)
                 }
                 switchMode(t) {
                     this.mode = t
                 }
                 beginGroup() {
                     this.macros.beginGroup()
                 }
@@ -14669,42 +14669,42 @@
                     for (; this.future().text === " ";) this.stack.pop()
                 }
                 consumeArg(t) {
                     let o = [],
                         s = t && t.length > 0;
                     s || this.consumeSpaces();
                     let u = this.future(),
-                        f, b = 0,
+                        p, b = 0,
                         v = 0;
                     do {
-                        if (f = this.popToken(), o.push(f), f.text === "{") ++b;
-                        else if (f.text === "}") {
-                            if (--b, b === -1) throw new a("Extra }", f)
-                        } else if (f.text === "EOF") throw new a("Unexpected end of input in a macro argument, expected '" + (t && s ? t[v] : "}") + "'", f);
+                        if (p = this.popToken(), o.push(p), p.text === "{") ++b;
+                        else if (p.text === "}") {
+                            if (--b, b === -1) throw new a("Extra }", p)
+                        } else if (p.text === "EOF") throw new a("Unexpected end of input in a macro argument, expected '" + (t && s ? t[v] : "}") + "'", p);
                         if (t && s)
-                            if ((b === 0 || b === 1 && t[v] === "{") && f.text === t[v]) {
+                            if ((b === 0 || b === 1 && t[v] === "{") && p.text === t[v]) {
                                 if (++v, v === t.length) {
                                     o.splice(-v, v);
                                     break
                                 }
                             } else v = 0
                     } while (b !== 0 || s);
                     return u.text === "{" && o[o.length - 1].text === "}" && (o.pop(), o.shift()), o.reverse(), {
                         tokens: o,
                         start: u,
-                        end: f
+                        end: p
                     }
                 }
                 consumeArgs(t, o) {
                     if (o) {
                         if (o.length !== t + 1) throw new a("The length of delimiters doesn't match the number of args!");
                         let u = o[0];
-                        for (let f = 0; f < u.length; f++) {
+                        for (let p = 0; p < u.length; p++) {
                             let b = this.popToken();
-                            if (u[f] !== b.text) throw new a("Use of the macro doesn't match its definition", b)
+                            if (u[p] !== b.text) throw new a("Use of the macro doesn't match its definition", b)
                         }
                     }
                     let s = [];
                     for (let u = 0; u < t; u++) s.push(this.consumeArg(o && o[u + 1]).tokens);
                     return s
                 }
                 countExpansion(t) {
@@ -14715,29 +14715,29 @@
                         s = o.text,
                         u = o.noexpand ? null : this._getExpansion(s);
                     if (u == null || t && u.unexpandable) {
                         if (t && u == null && s[0] === "\\" && !this.isDefined(s)) throw new a("Undefined control sequence: " + s);
                         return this.pushToken(o), !1
                     }
                     this.countExpansion(1);
-                    let f = u.tokens,
+                    let p = u.tokens,
                         b = this.consumeArgs(u.numArgs, u.delimiters);
                     if (u.numArgs) {
-                        f = f.slice();
-                        for (let v = f.length - 1; v >= 0; --v) {
-                            let S = f[v];
+                        p = p.slice();
+                        for (let v = p.length - 1; v >= 0; --v) {
+                            let S = p[v];
                             if (S.text === "#") {
                                 if (v === 0) throw new a("Incomplete placeholder at end of macro body", S);
-                                if (S = f[--v], S.text === "#") f.splice(v + 1, 1);
-                                else if (/^[1-9]$/.test(S.text)) f.splice(v, 2, ...b[+S.text - 1]);
+                                if (S = p[--v], S.text === "#") p.splice(v + 1, 1);
+                                else if (/^[1-9]$/.test(S.text)) p.splice(v, 2, ...b[+S.text - 1]);
                                 else throw new a("Not a valid argument number", S)
                             }
                         }
                     }
-                    return this.pushTokens(f), f.length
+                    return this.pushTokens(p), p.length
                 }
                 expandAfterFuture() {
                     return this.expandOnce(), this.future()
                 }
                 expandNextToken() {
                     for (;;)
                         if (this.expandOnce() === !1) {
@@ -14771,35 +14771,35 @@
                     let s = typeof o == "function" ? o(this) : o;
                     if (typeof s == "string") {
                         let u = 0;
                         if (s.indexOf("#") !== -1) {
                             let E = s.replace(/##/g, "");
                             for (; E.indexOf("#" + (u + 1)) !== -1;) ++u
                         }
-                        let f = new Ho(s, this.settings),
+                        let p = new jo(s, this.settings),
                             b = [],
-                            v = f.lex();
-                        for (; v.text !== "EOF";) b.push(v), v = f.lex();
+                            v = p.lex();
+                        for (; v.text !== "EOF";) b.push(v), v = p.lex();
                         return b.reverse(), {
                             tokens: b,
                             numArgs: u
                         }
                     }
                     return s
                 }
                 isDefined(t) {
-                    return this.macros.has(t) || Gt.hasOwnProperty(t) || Oe.math.hasOwnProperty(t) || Oe.text.hasOwnProperty(t) || Uo.hasOwnProperty(t)
+                    return this.macros.has(t) || Gt.hasOwnProperty(t) || Oe.math.hasOwnProperty(t) || Oe.text.hasOwnProperty(t) || Qo.hasOwnProperty(t)
                 }
                 isExpandable(t) {
                     let o = this.macros.get(t);
                     return o != null ? typeof o == "string" || typeof o == "function" || !o.unexpandable : Gt.hasOwnProperty(t) && !Gt[t].primitive
                 }
             }
-            let Wo = /^[₊₋₌₍₎₀₁₂₃₄₅₆₇₈₉ₐₑₕᵢⱼₖₗₘₙₒₚᵣₛₜᵤᵥₓᵦᵧᵨᵩᵪ]/,
-                i0 = Object.freeze({
+            let Xo = /^[₊₋₌₍₎₀₁₂₃₄₅₆₇₈₉ₐₑₕᵢⱼₖₗₘₙₒₚᵣₛₜᵤᵥₓᵦᵧᵨᵩᵪ]/,
+                o0 = Object.freeze({
                     "\u208A": "+",
                     "\u208B": "-",
                     "\u208C": "=",
                     "\u208D": "(",
                     "\u208E": ")",
                     "\u2080": "0",
                     "\u2081": "1",
@@ -14895,15 +14895,15 @@
                     "\u1D5D": "\u03B2",
                     "\u1D5E": "\u03B3",
                     "\u1D5F": "\u03B4",
                     "\u1D60": "\u03D5",
                     "\u1D61": "\u03C7",
                     "\u1DBF": "\u03B8"
                 }),
-                Cn = {
+                Tn = {
                     "\u0301": {
                         text: "\\'",
                         math: "\\acute"
                     },
                     "\u0300": {
                         text: "\\`",
                         math: "\\grave"
@@ -14943,15 +14943,15 @@
                     "\u030B": {
                         text: "\\H"
                     },
                     "\u0327": {
                         text: "\\c"
                     }
                 },
-                Yo = {
+                Jo = {
                     \u00E1: "a\u0301",
                     \u00E0: "a\u0300",
                     \u00E4: "a\u0308",
                     \u01DF: "a\u0308\u0304",
                     \u00E3: "a\u0303",
                     \u0101: "a\u0304",
                     \u0103: "a\u0306",
@@ -15289,17 +15289,17 @@
                     \u1FEA: "\u03A5\u0300",
                     \u03AB: "\u03A5\u0308",
                     \u1FE9: "\u03A5\u0304",
                     \u1FE8: "\u03A5\u0306",
                     \u038F: "\u03A9\u0301",
                     \u1FFA: "\u03A9\u0300"
                 };
-            class o0 {
+            class a0 {
                 constructor(t, o) {
-                    this.mode = void 0, this.gullet = void 0, this.settings = void 0, this.leftrightDepth = void 0, this.nextToken = void 0, this.mode = "math", this.gullet = new Y1(t, o, this.mode), this.settings = o, this.leftrightDepth = 0
+                    this.mode = void 0, this.gullet = void 0, this.settings = void 0, this.leftrightDepth = void 0, this.nextToken = void 0, this.mode = "math", this.gullet = new Z1(t, o, this.mode), this.settings = o, this.leftrightDepth = 0
                 }
                 expect(t, o) {
                     if (o === void 0 && (o = !0), this.fetch().text !== t) throw new a("Expected '" + t + "', got '" + this.fetch().text + "'", this.fetch());
                     o && this.consume()
                 }
                 consume() {
                     this.nextToken = null
@@ -15326,60 +15326,60 @@
                     return this.expect("}"), this.nextToken = o, s
                 }
                 parseExpression(t, o) {
                     let s = [];
                     for (;;) {
                         this.mode === "math" && this.consumeSpaces();
                         let u = this.fetch();
-                        if (o0.endOfExpression.indexOf(u.text) !== -1 || o && u.text === o || t && Gt[u.text] && Gt[u.text].infix) break;
-                        let f = this.parseAtom(o);
-                        if (f) {
-                            if (f.type === "internal") continue
+                        if (a0.endOfExpression.indexOf(u.text) !== -1 || o && u.text === o || t && Gt[u.text] && Gt[u.text].infix) break;
+                        let p = this.parseAtom(o);
+                        if (p) {
+                            if (p.type === "internal") continue
                         } else break;
-                        s.push(f)
+                        s.push(p)
                     }
                     return this.mode === "text" && this.formLigatures(s), this.handleInfixNodes(s)
                 }
                 handleInfixNodes(t) {
                     let o = -1,
                         s;
                     for (let u = 0; u < t.length; u++)
                         if (t[u].type === "infix") {
                             if (o !== -1) throw new a("only one infix operator per group", t[u].token);
                             o = u, s = t[u].replaceWith
                         } if (o !== -1 && s) {
-                        let u, f, b = t.slice(0, o),
+                        let u, p, b = t.slice(0, o),
                             v = t.slice(o + 1);
                         b.length === 1 && b[0].type === "ordgroup" ? u = b[0] : u = {
                             type: "ordgroup",
                             mode: this.mode,
                             body: b
-                        }, v.length === 1 && v[0].type === "ordgroup" ? f = v[0] : f = {
+                        }, v.length === 1 && v[0].type === "ordgroup" ? p = v[0] : p = {
                             type: "ordgroup",
                             mode: this.mode,
                             body: v
                         };
                         let S;
-                        return s === "\\\\abovefrac" ? S = this.callFunction(s, [u, t[o], f], []) : S = this.callFunction(s, [u, f], []), [S]
+                        return s === "\\\\abovefrac" ? S = this.callFunction(s, [u, t[o], p], []) : S = this.callFunction(s, [u, p], []), [S]
                     } else return t
                 }
                 handleSupSubscript(t) {
                     let o = this.fetch(),
                         s = o.text;
                     this.consume(), this.consumeSpaces();
                     let u = this.parseGroup(t);
                     if (!u) throw new a("Expected group after '" + s + "'", o);
                     return u
                 }
                 formatUnsupportedCmd(t) {
                     let o = [];
-                    for (let f = 0; f < t.length; f++) o.push({
+                    for (let p = 0; p < t.length; p++) o.push({
                         type: "textord",
                         mode: "text",
-                        text: t[f]
+                        text: t[p]
                     });
                     let s = {
                         type: "text",
                         mode: this.mode,
                         body: o
                     };
                     return {
@@ -15391,49 +15391,49 @@
                 }
                 parseAtom(t) {
                     let o = this.parseGroup("atom", t);
                     if (this.mode === "text") return o;
                     let s, u;
                     for (;;) {
                         this.consumeSpaces();
-                        let f = this.fetch();
-                        if (f.text === "\\limits" || f.text === "\\nolimits") {
+                        let p = this.fetch();
+                        if (p.text === "\\limits" || p.text === "\\nolimits") {
                             if (o && o.type === "op") {
-                                let b = f.text === "\\limits";
+                                let b = p.text === "\\limits";
                                 o.limits = b, o.alwaysHandleSupSub = !0
-                            } else if (o && o.type === "operatorname") o.alwaysHandleSupSub && (o.limits = f.text === "\\limits");
-                            else throw new a("Limit controls must follow a math operator", f);
+                            } else if (o && o.type === "operatorname") o.alwaysHandleSupSub && (o.limits = p.text === "\\limits");
+                            else throw new a("Limit controls must follow a math operator", p);
                             this.consume()
-                        } else if (f.text === "^") {
-                            if (s) throw new a("Double superscript", f);
+                        } else if (p.text === "^") {
+                            if (s) throw new a("Double superscript", p);
                             s = this.handleSupSubscript("superscript")
-                        } else if (f.text === "_") {
-                            if (u) throw new a("Double subscript", f);
+                        } else if (p.text === "_") {
+                            if (u) throw new a("Double subscript", p);
                             u = this.handleSupSubscript("subscript")
-                        } else if (f.text === "'") {
-                            if (s) throw new a("Double superscript", f);
+                        } else if (p.text === "'") {
+                            if (s) throw new a("Double superscript", p);
                             let b = {
                                     type: "textord",
                                     mode: this.mode,
                                     text: "\\prime"
                                 },
                                 v = [b];
                             for (this.consume(); this.fetch().text === "'";) v.push(b), this.consume();
                             this.fetch().text === "^" && v.push(this.handleSupSubscript("superscript")), s = {
                                 type: "ordgroup",
                                 mode: this.mode,
                                 body: v
                             }
-                        } else if (i0[f.text]) {
-                            let b = Wo.test(f.text),
+                        } else if (o0[p.text]) {
+                            let b = Xo.test(p.text),
                                 v = [];
-                            for (v.push(new mt(i0[f.text])), this.consume();;) {
+                            for (v.push(new mt(o0[p.text])), this.consume();;) {
                                 let E = this.fetch().text;
-                                if (!i0[E] || Wo.test(E) !== b) break;
-                                v.unshift(new mt(i0[E])), this.consume()
+                                if (!o0[E] || Xo.test(E) !== b) break;
+                                v.unshift(new mt(o0[E])), this.consume()
                             }
                             let S = this.subparse(v);
                             b ? u = {
                                 type: "ordgroup",
                                 mode: "math",
                                 body: S
                             } : s = {
@@ -15450,56 +15450,56 @@
                         sup: s,
                         sub: u
                     } : o
                 }
                 parseFunction(t, o) {
                     let s = this.fetch(),
                         u = s.text,
-                        f = Gt[u];
-                    if (!f) return null;
-                    if (this.consume(), o && o !== "atom" && !f.allowedInArgument) throw new a("Got function '" + u + "' with no arguments" + (o ? " as " + o : ""), s);
-                    if (this.mode === "text" && !f.allowedInText) throw new a("Can't use function '" + u + "' in text mode", s);
-                    if (this.mode === "math" && f.allowedInMath === !1) throw new a("Can't use function '" + u + "' in math mode", s);
+                        p = Gt[u];
+                    if (!p) return null;
+                    if (this.consume(), o && o !== "atom" && !p.allowedInArgument) throw new a("Got function '" + u + "' with no arguments" + (o ? " as " + o : ""), s);
+                    if (this.mode === "text" && !p.allowedInText) throw new a("Can't use function '" + u + "' in text mode", s);
+                    if (this.mode === "math" && p.allowedInMath === !1) throw new a("Can't use function '" + u + "' in math mode", s);
                     let {
                         args: b,
                         optArgs: v
-                    } = this.parseArguments(u, f);
+                    } = this.parseArguments(u, p);
                     return this.callFunction(u, b, v, s, t)
                 }
-                callFunction(t, o, s, u, f) {
+                callFunction(t, o, s, u, p) {
                     let b = {
                             funcName: t,
                             parser: this,
                             token: u,
-                            breakOnTokenText: f
+                            breakOnTokenText: p
                         },
                         v = Gt[t];
                     if (v && v.handler) return v.handler(b, o, s);
                     throw new a("No function handler for " + t)
                 }
                 parseArguments(t, o) {
                     let s = o.numArgs + o.numOptionalArgs;
                     if (s === 0) return {
                         args: [],
                         optArgs: []
                     };
                     let u = [],
-                        f = [];
+                        p = [];
                     for (let b = 0; b < s; b++) {
                         let v = o.argTypes && o.argTypes[b],
                             S = b < o.numOptionalArgs;
-                        (o.primitive && v == null || o.type === "sqrt" && b === 1 && f[0] == null) && (v = "primitive");
+                        (o.primitive && v == null || o.type === "sqrt" && b === 1 && p[0] == null) && (v = "primitive");
                         let E = this.parseGroupOfType("argument to '" + t + "'", v, S);
-                        if (S) f.push(E);
+                        if (S) p.push(E);
                         else if (E != null) u.push(E);
                         else throw new a("Null argument, please report this as a bug")
                     }
                     return {
                         args: u,
-                        optArgs: f
+                        optArgs: p
                     }
                 }
                 parseGroupOfType(t, o, s) {
                     switch (o) {
                         case "color":
                             return this.parseColorGroup(s);
                         case "size":
@@ -15543,28 +15543,28 @@
                 consumeSpaces() {
                     for (; this.fetch().text === " ";) this.consume()
                 }
                 parseStringGroup(t, o) {
                     let s = this.gullet.scanArgument(o);
                     if (s == null) return null;
                     let u = "",
-                        f;
+                        p;
                     for (;
-                        (f = this.fetch()).text !== "EOF";) u += f.text, this.consume();
+                        (p = this.fetch()).text !== "EOF";) u += p.text, this.consume();
                     return this.consume(), s.text = u, s
                 }
                 parseRegexGroup(t, o) {
                     let s = this.fetch(),
                         u = s,
-                        f = "",
+                        p = "",
                         b;
                     for (;
-                        (b = this.fetch()).text !== "EOF" && t.test(f + b.text);) u = b, f += u.text, this.consume();
-                    if (f === "") throw new a("Invalid " + o + ": '" + s.text + "'", s);
-                    return s.range(u, f)
+                        (b = this.fetch()).text !== "EOF" && t.test(p + b.text);) u = b, p += u.text, this.consume();
+                    if (p === "") throw new a("Invalid " + o + ": '" + s.text + "'", s);
+                    return s.range(u, p)
                 }
                 parseColorGroup(t) {
                     let o = this.parseStringGroup("color", t);
                     if (o == null) return null;
                     let s = /^(#[a-f0-9]{3}|#?[a-f0-9]{6}|[a-z]+)$/i.exec(o.text);
                     if (!s) throw new a("Invalid color: '" + o.text + "'", o);
                     let u = s[0];
@@ -15576,23 +15576,23 @@
                 }
                 parseSizeGroup(t) {
                     let o, s = !1;
                     if (this.gullet.consumeSpaces(), !t && this.gullet.future().text !== "{" ? o = this.parseRegexGroup(/^[-+]? *(?:$|\d+|\d+\.\d*|\.\d*) *[a-z]{0,2} *$/, "size") : o = this.parseStringGroup("size", t), !o) return null;
                     !t && o.text.length === 0 && (o.text = "0pt", s = !0);
                     let u = /([-+]?) *(\d+(?:\.\d*)?|\.\d+) *([a-z]{2})/.exec(o.text);
                     if (!u) throw new a("Invalid size: '" + o.text + "'", o);
-                    let f = {
+                    let p = {
                         number: +(u[1] + u[2]),
                         unit: u[3]
                     };
-                    if (!Ei(f)) throw new a("Invalid unit: '" + f.unit + "'", o);
+                    if (!Fi(p)) throw new a("Invalid unit: '" + p.unit + "'", o);
                     return {
                         type: "size",
                         mode: this.mode,
-                        value: f,
+                        value: p,
                         isBlank: s
                     }
                 }
                 parseUrlGroup(t) {
                     this.gullet.lexer.setCatcode("%", 13), this.gullet.lexer.setCatcode("~", 12);
                     let o = this.parseStringGroup("url", t);
                     if (this.gullet.lexer.setCatcode("%", 14), this.gullet.lexer.setCatcode("~", 13), o == null) return null;
@@ -15604,734 +15604,739 @@
                     }
                 }
                 parseArgumentGroup(t, o) {
                     let s = this.gullet.scanArgument(t);
                     if (s == null) return null;
                     let u = this.mode;
                     o && this.switchMode(o), this.gullet.beginGroup();
-                    let f = this.parseExpression(!1, "EOF");
+                    let p = this.parseExpression(!1, "EOF");
                     this.expect("EOF"), this.gullet.endGroup();
                     let b = {
                         type: "ordgroup",
                         mode: this.mode,
                         loc: s.loc,
-                        body: f
+                        body: p
                     };
                     return o && this.switchMode(u), b
                 }
                 parseGroup(t, o) {
                     let s = this.fetch(),
                         u = s.text,
-                        f;
+                        p;
                     if (u === "{" || u === "\\begingroup") {
                         this.consume();
                         let b = u === "{" ? "}" : "\\endgroup";
                         this.gullet.beginGroup();
                         let v = this.parseExpression(!1, b),
                             S = this.fetch();
-                        this.expect(b), this.gullet.endGroup(), f = {
+                        this.expect(b), this.gullet.endGroup(), p = {
                             type: "ordgroup",
                             mode: this.mode,
                             loc: st.range(s, S),
                             body: v,
                             semisimple: u === "\\begingroup" || void 0
                         }
-                    } else if (f = this.parseFunction(o, t) || this.parseSymbol(), f == null && u[0] === "\\" && !Uo.hasOwnProperty(u)) {
+                    } else if (p = this.parseFunction(o, t) || this.parseSymbol(), p == null && u[0] === "\\" && !Qo.hasOwnProperty(u)) {
                         if (this.settings.throwOnError) throw new a("Undefined control sequence: " + u, s);
-                        f = this.formatUnsupportedCmd(u), this.consume()
+                        p = this.formatUnsupportedCmd(u), this.consume()
                     }
-                    return f
+                    return p
                 }
                 formLigatures(t) {
                     let o = t.length - 1;
                     for (let s = 0; s < o; ++s) {
                         let u = t[s],
-                            f = u.text;
-                        f === "-" && t[s + 1].text === "-" && (s + 1 < o && t[s + 2].text === "-" ? (t.splice(s, 3, {
+                            p = u.text;
+                        p === "-" && t[s + 1].text === "-" && (s + 1 < o && t[s + 2].text === "-" ? (t.splice(s, 3, {
                             type: "textord",
                             mode: "text",
                             loc: st.range(u, t[s + 2]),
                             text: "---"
                         }), o -= 2) : (t.splice(s, 2, {
                             type: "textord",
                             mode: "text",
                             loc: st.range(u, t[s + 1]),
                             text: "--"
-                        }), o -= 1)), (f === "'" || f === "`") && t[s + 1].text === f && (t.splice(s, 2, {
+                        }), o -= 1)), (p === "'" || p === "`") && t[s + 1].text === p && (t.splice(s, 2, {
                             type: "textord",
                             mode: "text",
                             loc: st.range(u, t[s + 1]),
-                            text: f + f
+                            text: p + p
                         }), o -= 1)
                     }
                 }
                 parseSymbol() {
                     let t = this.fetch(),
                         o = t.text;
                     if (/^\\verb[^a-zA-Z]/.test(o)) {
                         this.consume();
-                        let f = o.slice(5),
-                            b = f.charAt(0) === "*";
-                        if (b && (f = f.slice(1)), f.length < 2 || f.charAt(0) !== f.slice(-1)) throw new a(`\\verb assertion failed --
+                        let p = o.slice(5),
+                            b = p.charAt(0) === "*";
+                        if (b && (p = p.slice(1)), p.length < 2 || p.charAt(0) !== p.slice(-1)) throw new a(`\\verb assertion failed --
                     please report what input caused this bug`);
-                        return f = f.slice(1, -1), {
+                        return p = p.slice(1, -1), {
                             type: "verb",
                             mode: "text",
-                            body: f,
+                            body: p,
                             star: b
                         }
                     }
-                    Yo.hasOwnProperty(o[0]) && !Oe[this.mode][o[0]] && (this.settings.strict && this.mode === "math" && this.settings.reportNonstrict("unicodeTextInMathMode", 'Accented Unicode text character "' + o[0] + '" used in math mode', t), o = Yo[o[0]] + o.slice(1));
-                    let s = V1.exec(o);
+                    Jo.hasOwnProperty(o[0]) && !Oe[this.mode][o[0]] && (this.settings.strict && this.mode === "math" && this.settings.reportNonstrict("unicodeTextInMathMode", 'Accented Unicode text character "' + o[0] + '" used in math mode', t), o = Jo[o[0]] + o.slice(1));
+                    let s = j1.exec(o);
                     s && (o = o.substring(0, s.index), o === "i" ? o = "\u0131" : o === "j" && (o = "\u0237"));
                     let u;
                     if (Oe[this.mode][o]) {
-                        this.settings.strict && this.mode === "math" && Y0.indexOf(o) >= 0 && this.settings.reportNonstrict("unicodeTextInMathMode", 'Latin-1/Unicode text character "' + o[0] + '" used in math mode', t);
-                        let f = Oe[this.mode][o].group,
+                        this.settings.strict && this.mode === "math" && Z0.indexOf(o) >= 0 && this.settings.reportNonstrict("unicodeTextInMathMode", 'Latin-1/Unicode text character "' + o[0] + '" used in math mode', t);
+                        let p = Oe[this.mode][o].group,
                             b = st.range(t),
                             v;
-                        if (Vu.hasOwnProperty(f)) {
-                            let S = f;
+                        if (ju.hasOwnProperty(p)) {
+                            let S = p;
                             v = {
                                 type: "atom",
                                 mode: this.mode,
                                 family: S,
                                 loc: b,
                                 text: o
                             }
                         } else v = {
-                            type: f,
+                            type: p,
                             mode: this.mode,
                             loc: b,
                             text: o
                         };
                         u = v
                     } else if (o.charCodeAt(0) >= 128) this.settings.strict && (qt(o.charCodeAt(0)) ? this.mode === "math" && this.settings.reportNonstrict("unicodeTextInMathMode", 'Unicode text character "' + o[0] + '" used in math mode', t) : this.settings.reportNonstrict("unknownSymbol", 'Unrecognized Unicode character "' + o[0] + '"' + (" (" + o.charCodeAt(0) + ")"), t)), u = {
                         type: "textord",
                         mode: "text",
                         loc: st.range(t),
                         text: o
                     };
                     else return null;
                     if (this.consume(), s)
-                        for (let f = 0; f < s[0].length; f++) {
-                            let b = s[0][f];
-                            if (!Cn[b]) throw new a("Unknown accent ' " + b + "'", t);
-                            let v = Cn[b][this.mode] || Cn[b].text;
+                        for (let p = 0; p < s[0].length; p++) {
+                            let b = s[0][p];
+                            if (!Tn[b]) throw new a("Unknown accent ' " + b + "'", t);
+                            let v = Tn[b][this.mode] || Tn[b].text;
                             if (!v) throw new a("Accent " + b + " unsupported in " + this.mode + " mode", t);
                             u = {
                                 type: "accent",
                                 mode: this.mode,
                                 loc: st.range(t),
                                 label: v,
                                 isStretchy: !1,
                                 isShifty: !0,
                                 base: u
                             }
                         }
                     return u
                 }
             }
-            o0.endOfExpression = ["}", "\\endgroup", "\\end", "\\right", "&"];
-            var Tn = function(n, t) {
+            a0.endOfExpression = ["}", "\\endgroup", "\\end", "\\right", "&"];
+            var An = function(n, t) {
                 if (!(typeof n == "string" || n instanceof String)) throw new TypeError("KaTeX can only parse string typed expression");
-                let o = new o0(n, t);
+                let o = new a0(n, t);
                 delete o.gullet.macros.current["\\df@tag"];
                 let s = o.parse();
                 if (delete o.gullet.macros.current["\\current@color"], delete o.gullet.macros.current["\\color"], o.gullet.macros.get("\\df@tag")) {
                     if (!t.displayMode) throw new a("\\tag works only in display equations");
                     s = [{
                         type: "tag",
                         mode: "text",
                         body: s,
                         tag: o.subparse([new mt("\\df@tag")])
                     }]
                 }
                 return s
             };
-            let Qo = function(n, t, o) {
+            let Ko = function(n, t, o) {
                 t.textContent = "";
-                let s = An(n, o).toNode();
+                let s = qn(n, o).toNode();
                 t.appendChild(s)
             };
-            typeof document < "u" && document.compatMode !== "CSS1Compat" && (typeof console < "u" && console.warn("Warning: KaTeX doesn't work in quirks mode. Make sure your website has a suitable doctype."), Qo = function() {
+            typeof document < "u" && document.compatMode !== "CSS1Compat" && (typeof console < "u" && console.warn("Warning: KaTeX doesn't work in quirks mode. Make sure your website has a suitable doctype."), Ko = function() {
                 throw new a("KaTeX doesn't work in quirks mode.")
             });
             let Q1 = function(n, t) {
-                    return An(n, t).toMarkup()
+                    return qn(n, t).toMarkup()
                 },
-                Z1 = function(n, t) {
+                X1 = function(n, t) {
                     let o = new I(t);
-                    return Tn(n, o)
+                    return An(n, o)
                 },
-                Zo = function(n, t, o) {
+                ea = function(n, t, o) {
                     if (o.throwOnError || !(n instanceof a)) throw n;
                     let s = B.makeSpan(["katex-error"], [new ut(t)]);
                     return s.setAttribute("title", n.toString()), s.setAttribute("style", "color:" + o.errorColor), s
                 },
-                An = function(n, t) {
+                qn = function(n, t) {
                     let o = new I(t);
                     try {
-                        let s = Tn(n, o);
-                        return h1(s, n, o)
+                        let s = An(n, o);
+                        return d1(s, n, o)
                     } catch (s) {
-                        return Zo(s, n, o)
+                        return ea(s, n, o)
                     }
                 };
-            var X1 = {
+            var J1 = {
                     version: "0.16.10",
-                    render: Qo,
+                    render: Ko,
                     renderToString: Q1,
                     ParseError: a,
-                    SETTINGS_SCHEMA: G,
-                    __parse: Z1,
-                    __renderToDomTree: An,
+                    SETTINGS_SCHEMA: O,
+                    __parse: X1,
+                    __renderToDomTree: qn,
                     __renderToHTMLTree: function(n, t) {
                         let o = new I(t);
                         try {
-                            let s = Tn(n, o);
-                            return d1(s, n, o)
+                            let s = An(n, o);
+                            return m1(s, n, o)
                         } catch (s) {
-                            return Zo(s, n, o)
+                            return ea(s, n, o)
                         }
                     },
-                    __setFontMetrics: Nu,
+                    __setFontMetrics: Lu,
                     __defineSymbol: h,
-                    __defineFunction: Z,
-                    __defineMacro: w,
+                    __defineFunction: Q,
+                    __defineMacro: k,
                     __domTree: {
                         Span: vr,
-                        Anchor: U0,
+                        Anchor: W0,
                         SymbolNode: ut,
                         SvgNode: Et,
                         PathNode: Ot,
-                        LineNode: W0
+                        LineNode: Y0
                     }
                 },
-                J1 = X1;
+                K1 = J1;
             return e = e.default, e
         }()
     })
 });
-var Cu = W((G2, Su) => {
+var Tu = W(Hr => {
     "use strict";
-    var yu = bu();
+    var Lp = Hr && Hr.__importDefault || function(r) {
+        return r && r.__esModule ? r : {
+            default: r
+        }
+    };
+    Object.defineProperty(Hr, "__esModule", {
+        value: !0
+    });
+    var vu = Lp(xu());
 
-    function xu(r, e) {
+    function wu(r, e) {
         let i = r.src[e - 1],
             a = r.src[e],
             l = r.src[e + 1];
         if (a !== "$") return {
             can_open: !1,
             can_close: !1
         };
         let c = !1,
             d = !1;
-        return i !== "$" && i !== "\\" && (i === void 0 || vu(i) || !wu(i)) && (c = !0), l !== "$" && (l == null || vu(l) || !wu(l)) && (d = !0), {
+        return i !== "$" && i !== "\\" && (i === void 0 || ku(i) || !_u(i)) && (c = !0), l !== "$" && (l == null || ku(l) || !_u(l)) && (d = !0), {
             can_open: c,
             can_close: d
         }
     }
 
-    function vu(r) {
+    function ku(r) {
         return /^\s$/u.test(r)
     }
 
-    function wu(r) {
+    function _u(r) {
         return /^[\w\d]$/u.test(r)
     }
 
-    function ku(r, e) {
+    function Su(r, e) {
         let i = r.src[e - 1],
             a = r.src[e],
             l = r.src[e + 1],
             c = r.src[e + 2];
         return a === "$" && i !== "$" && i !== "\\" && l === "$" && c !== "$" ? {
             can_open: !0,
             can_close: !0
         } : {
             can_open: !1,
             can_close: !1
         }
     }
 
-    function Rp(r, e) {
+    function Pp(r, e) {
         if (r.src[r.pos] !== "$") return !1;
         let i = r.tokens.at(-1);
-        if (i?.type === "html_inline" && /^<\w+.+[^/]>$/.test(i.content)) return;
-        let a = xu(r, r.pos);
+        if (i?.type === "html_inline" && /^<\w+.+[^/]>$/.test(i.content)) return !1;
+        let a = wu(r, r.pos);
         if (!a.can_open) return e || (r.pending += "$"), r.pos += 1, !0;
         let l = r.pos + 1,
             c = l,
             d;
         for (;
             (c = r.src.indexOf("$", c)) !== -1;) {
             for (d = c - 1; r.src[d] === "\\";) d -= 1;
             if ((c - d) % 2 == 1) break;
             c += 1
         }
         if (c === -1) return e || (r.pending += "$"), r.pos = l, !0;
         if (c - l === 0) return e || (r.pending += "$$"), r.pos = l + 1, !0;
-        if (a = xu(r, c), !a.can_close) return e || (r.pending += "$"), r.pos = l, !0;
+        if (a = wu(r, c), !a.can_close) return e || (r.pending += "$"), r.pos = l, !0;
         if (!e) {
-            let m = r.push("math_inline", "math", 0);
-            m.markup = "$", m.content = r.src.slice(l, c)
+            let f = r.push("math_inline", "math", 0);
+            f.markup = "$", f.content = r.src.slice(l, c)
         }
         return r.pos = c + 1, !0
     }
 
-    function Fp(r, e, i, a) {
-        var l, c, d, m = !1,
+    function Ip(r, e, i, a) {
+        var l, c, d, f = !1,
             g, y = r.bMarks[e] + r.tShift[e],
             _ = r.eMarks[e];
         if (y + 2 > _ || r.src.slice(y, y + 2) !== "$$") return !1;
         y += 2;
-        let k = r.src.slice(y, _);
+        let w = r.src.slice(y, _);
         if (a) return !0;
-        for (k.trim().slice(-2) === "$$" && (k = k.trim().slice(0, -2), m = !0), c = e; !m && (c++, !(c >= i || (y = r.bMarks[c] + r.tShift[c], _ = r.eMarks[c], y < _ && r.tShift[c] < r.blkIndent)));) r.src.slice(y, _).trim().slice(-2) === "$$" ? (d = r.src.slice(0, _).lastIndexOf("$$"), l = r.src.slice(y, d), m = !0) : r.src.slice(y, _).trim().includes("$$") && (d = r.src.slice(0, _).trim().indexOf("$$"), l = r.src.slice(y, d), m = !0);
-        return r.line = c + 1, g = r.push("math_block", "math", 0), g.block = !0, g.content = (k && k.trim() ? k + `
+        for (w.trim().slice(-2) === "$$" && (w = w.trim().slice(0, -2), f = !0), c = e; !f && (c++, !(c >= i || (y = r.bMarks[c] + r.tShift[c], _ = r.eMarks[c], y < _ && r.tShift[c] < r.blkIndent)));) r.src.slice(y, _).trim().slice(-2) === "$$" ? (d = r.src.slice(0, _).lastIndexOf("$$"), l = r.src.slice(y, d), f = !0) : r.src.slice(y, _).trim().includes("$$") && (d = r.src.slice(0, _).trim().indexOf("$$"), l = r.src.slice(y, d), f = !0);
+        return r.line = c + 1, g = r.push("math_block", "math", 0), g.block = !0, g.content = (w && w.trim() ? w + `
 ` : "") + r.getLines(e + 1, c, r.tShift[e], !0) + (l && l.trim() ? l : ""), g.map = [e, r.line], g.markup = "$$", !0
     }
 
-    function Bp(r, e, i, a) {
-        var l, c = !1,
-            d = r.bMarks[e] + r.tShift[e],
-            m = r.eMarks[e];
-        let g = r.src.slice(d, m);
-        if (!/^\\begin/.test(g)) return !1;
+    function Op(r, e, i, a) {
+        let l = r.bMarks[e] + r.tShift[e],
+            c = r.eMarks[e];
+        if (!r.src.slice(l, c).match(/^\s*\\begin\s*\{([^{}]+)\}/)) return !1;
         if (e > 0) {
-            let k = r.bMarks[e - 1] + r.tShift[e - 1],
-                T = r.eMarks[e - 1],
-                A = r.src.slice(k, T);
-            if (!/^\s*$/.test(A)) return !1
+            let A = r.bMarks[e - 1] + r.tShift[e - 1],
+                L = r.eMarks[e - 1],
+                R = r.src.slice(A, L);
+            if (!/^\s*$/.test(R)) return !1
         }
         if (a) return !0;
-        let y = e;
-        if (!/\\end[\{\}\w]*\s*$/.test(g)) {
-            let k = 0;
-            for (; !c && (y++, !(y >= i || (d = r.bMarks[y] + r.tShift[y], m = r.eMarks[y], d < m && r.tShift[y] < r.blkIndent)));) {
-                let T = r.src.slice(d, m);
-                if (/\\begin/.test(T)) ++k;
-                else if (/\\end/.test(T) && (--k, k < 0)) {
-                    let A = m;
-                    l = r.src.slice(d, A), c = !0
-                }
+        let g = [],
+            y = e,
+            _, w = !1;
+        e: for (; !w && !(y >= i); y++) {
+            let A = r.bMarks[y] + r.tShift[y],
+                L = r.eMarks[y];
+            if (A < L && r.tShift[y] < r.blkIndent) break;
+            let R = r.src.slice(A, L);
+            for (let O of R.matchAll(/(\\begin|\\end)\s*\{([^{}]+)\}/g))
+                if (O[1] === "\\begin") g.push(O[2].trim());
+                else if (O[1] === "\\end" && (g.pop(), !g.length)) {
+                _ = r.src.slice(A, L), w = !0;
+                break e
             }
         }
         r.line = y + 1;
-        let _ = r.push("math_block", "math", 0);
-        return _.block = !0, _.content = (g && g.trim() ? g + `
-` : "") + r.getLines(e + 1, y, r.tShift[e], !0) + (l && l.trim() ? l : ""), _.map = [e, r.line], _.markup = "$$", !0
+        let T = r.push("math_block", "math", 0);
+        return T.block = !0, T.content = (r.getLines(e, y, r.tShift[e], !0) + (_ ?? "")).trim(), T.map = [e, r.line], T.markup = "$$", !0
     }
 
-    function Np(r, e) {
+    function Hp(r, e) {
         var i, a, l, c, d;
         if (r.src.slice(r.pos, r.pos + 2) !== "$$") return !1;
-        if (c = ku(r, r.pos), !c.can_open) return e || (r.pending += "$$"), r.pos += 2, !0;
+        if (c = Su(r, r.pos), !c.can_open) return e || (r.pending += "$$"), r.pos += 2, !0;
         for (i = r.pos + 2, a = i;
             (a = r.src.indexOf("$$", a)) !== -1;) {
             for (d = a - 1; r.src[d] === "\\";) d -= 1;
             if ((a - d) % 2 == 1) break;
             a += 2
         }
-        return a === -1 ? (e || (r.pending += "$$"), r.pos = i, !0) : a - i === 0 ? (e || (r.pending += "$$$$"), r.pos = i + 2, !0) : (c = ku(r, a), c.can_close ? (e || (l = r.push("math_block", "math", 0), l.block = !0, l.markup = "$$", l.content = r.src.slice(i, a)), r.pos = a + 2, !0) : (e || (r.pending += "$$"), r.pos = i, !0))
+        return a === -1 ? (e || (r.pending += "$$"), r.pos = i, !0) : a - i === 0 ? (e || (r.pending += "$$$$"), r.pos = i + 2, !0) : (c = Su(r, a), c.can_close ? (e || (l = r.push("math_block", "math", 0), l.block = !0, l.markup = "$$", l.content = r.src.slice(i, a)), r.pos = a + 2, !0) : (e || (r.pending += "$$"), r.pos = i, !0))
     }
 
-    function Lp(r, e) {
-        let i = r.src.slice(r.pos, r.maxPos);
+    function $p(r, e) {
+        let i = r.src.slice(r.pos);
         if (!/^\n\\begin/.test(i)) return !1;
         if (r.pos += 1, e) return !0;
         let a = i.split(/\n/g).slice(1),
-            l = /^\\begin/,
-            c = /^\\end/,
-            d = 0,
-            m;
-        for (var g = 0; g < a.length; ++g) {
-            let _ = a[g];
-            if (l.test(_)) ++d;
-            else if (c.test(_) && (--d, d <= 0)) {
-                m = g;
-                break
+            l, c = [];
+        e: for (var d = 0; d < a.length; ++d) {
+            let y = a[d];
+            for (let _ of y.matchAll(/(\\begin|\\end)\s*\{([^{}]+)\}/g))
+                if (_[1] === "\\begin") c.push(_[2].trim());
+                else if (_[1] === "\\end" && (c.pop(), !c.length)) {
+                l = d;
+                break e
             }
         }
-        if (typeof m > "u") return !1;
-        let y = a.slice(0, m + 1).reduce((_, k) => _ + k.length, 0) + m + 1;
-        if (!e) {
-            let _ = r.push("math_inline_bare_block", "math", 0);
-            _.block = !0, _.markup = "$$", _.content = i.slice(1, y)
-        }
-        return r.pos = r.pos + y, !0
+        if (typeof l > "u") return !1;
+        let f = a.slice(0, l + 1).reduce((y, _) => y + _.length, 0) + l + 1,
+            g = r.push("math_inline_bare_block", "math", 0);
+        return g.block = !0, g.markup = "$$", g.content = i.slice(1, f), r.pos = r.pos + f, !0
     }
 
-    function _u(r, e, i, a) {
+    function Cu(r, e, i, a) {
         let l = r.tokens;
         for (let c = l.length - 1; c >= 0; c--) {
             let d = l[c],
-                m = [];
+                f = [];
             if (d.type !== "html_block") continue;
             let g = d.content;
             for (let y of g.matchAll(a)) {
+                if (!y.groups) continue;
                 let _ = y.groups.html_before_math,
-                    k = y.groups.math,
+                    w = y.groups.math,
                     T = y.groups.html_after_math;
-                _ && m.push({
+                _ && f.push({
                     ...d,
                     type: "html_block",
                     map: null,
                     content: _
-                }), k && m.push({
+                }), w && f.push({
                     ...d,
                     type: e,
                     map: null,
-                    content: k,
+                    content: w,
                     markup: i,
                     block: !0,
                     tag: "math"
-                }), T && m.push({
+                }), T && f.push({
                     ...d,
                     type: "html_block",
                     map: null,
                     content: T
                 })
             }
-            m.length > 0 && l.splice(c, 1, ...m)
+            f.length > 0 && l.splice(c, 1, ...f)
         }
         return !0
     }
 
-    function I0(r) {
+    function O0(r) {
         return r.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;").replace(/'/g, "&#039;")
     }
-    Su.exports = function(e, i) {
-        i = i || {};
-        let a = i.enableBareBlocks,
-            l = i.enableMathBlockInHtml,
-            c = i.enableMathInlineInHtml,
-            d = T => {
-                let A = /\\begin\{(align|equation|gather|cd|alignat)\}/ig.test(T);
+
+    function Gp(r, e) {
+        let i = e?.enableBareBlocks,
+            a = e?.enableMathBlockInHtml,
+            l = e?.enableMathInlineInHtml,
+            c = w => {
+                let T = /\\begin\{(align|equation|gather|cd|alignat)\}/ig.test(w);
                 try {
-                    return yu.renderToString(T, {
-                        ...i,
-                        displayMode: A
+                    return vu.default.renderToString(w, {
+                        ...e,
+                        displayMode: T
                     })
-                } catch (L) {
-                    return i.throwOnError && console.log(L), `<span class="katex-error" title="${I0(T)}">${I0(L.toString())}</span>`
+                } catch (A) {
+                    return e?.throwOnError && console.log(A), `<span class="katex-error" title="${O0(w)}">${O0(A+"")}</span>`
                 }
             },
-            m = (T, A) => d(T[A].content),
-            g = T => {
+            d = (w, T) => c(w[T].content),
+            f = w => {
                 try {
-                    return `<p class="katex-block">${yu.renderToString(T,{...i,displayMode:!0})}</p>`
-                } catch (A) {
-                    return i.throwOnError && console.log(A), `<p class="katex-block katex-error" title="${I0(T)}">${I0(A.toString())}</p>`
+                    return `<p class="katex-block">${vu.default.renderToString(w,{...e,displayMode:!0})}</p>`
+                } catch (T) {
+                    return e?.throwOnError && console.log(T), `<p class="katex-block katex-error" title="${O0(w)}">${O0(T+"")}</p>`
                 }
             },
-            y = (T, A) => g(T[A].content) + `
+            g = (w, T) => f(w[T].content) + `
 `;
-        e.inline.ruler.after("escape", "math_inline", Rp), e.inline.ruler.after("escape", "math_inline_block", Np), a && e.inline.ruler.before("text", "math_inline_bare_block", Lp), e.block.ruler.after("blockquote", "math_block", (T, A, L, R) => a && Bp(T, A, L, R) ? !0 : Fp(T, A, L, R), {
+        r.inline.ruler.after("escape", "math_inline", Pp), r.inline.ruler.after("escape", "math_inline_block", Hp), i && r.inline.ruler.before("text", "math_inline_bare_block", $p), r.block.ruler.after("blockquote", "math_block", (w, T, A, L) => i && Op(w, T, A, L) ? !0 : Ip(w, T, A, L), {
             alt: ["paragraph", "reference", "blockquote", "list"]
         });
-        let _ = /(?<html_before_math>[\s\S]*?)\$\$(?<math>[\s\S]+?)\$\$(?<html_after_math>(?:(?!\$\$[\s\S]+?\$\$)[\s\S])*)/gm,
-            k = /(?<html_before_math>[\s\S]*?)\$(?<math>.*?)\$(?<html_after_math>(?:(?!\$.*?\$)[\s\S])*)/gm;
-        l && e.core.ruler.push("math_block_in_html_block", T => _u(T, "math_block", "$$", _)), c && e.core.ruler.push("math_inline_in_html_block", T => _u(T, "math_inline", "$", k)), e.renderer.rules.math_inline = m, e.renderer.rules.math_inline_block = y, e.renderer.rules.math_inline_bare_block = y, e.renderer.rules.math_block = y
-    }
-});
-var h0, Me, oa, sh, Kt, ea, aa, Mn, lh, Tr = {},
-    sa = [],
-    ch = /acit|ex(?:s|g|n|p|$)|rph|grid|ows|mnc|ntw|ine[ch]|zoo|^ord|itera/i,
-    Dn = Array.isArray;
+        let y = /(?<html_before_math>[\s\S]*?)\$\$(?<math>[\s\S]+?)\$\$(?<html_after_math>(?:(?!\$\$[\s\S]+?\$\$)[\s\S])*)/gm,
+            _ = /(?<html_before_math>[\s\S]*?)\$(?<math>.*?)\$(?<html_after_math>(?:(?!\$.*?\$)[\s\S])*)/gm;
+        a && r.core.ruler.push("math_block_in_html_block", w => Cu(w, "math_block", "$$", y)), l && r.core.ruler.push("math_inline_in_html_block", w => Cu(w, "math_inline", "$", _)), r.renderer.rules.math_inline = d, r.renderer.rules.math_inline_block = g, r.renderer.rules.math_inline_bare_block = g, r.renderer.rules.math_block = g
+    }
+    Hr.default = Gp
+});
+var d0, Me, ca, lh, er, ia, ua, En, ch, Tr = {},
+    ha = [],
+    uh = /acit|ex(?:s|g|n|p|$)|rph|grid|ows|mnc|ntw|ine[ch]|zoo|^ord|itera/i,
+    zn = Array.isArray;
 
 function Vt(r, e) {
     for (var i in e) r[i] = e[i];
     return r
 }
 
-function la(r) {
+function da(r) {
     var e = r.parentNode;
     e && e.removeChild(r)
 }
 
-function uh(r, e, i) {
+function hh(r, e, i) {
     var a, l, c, d = {};
     for (c in e) c == "key" ? a = e[c] : c == "ref" ? l = e[c] : d[c] = e[c];
-    if (arguments.length > 2 && (d.children = arguments.length > 3 ? h0.call(arguments, 2) : i), typeof r == "function" && r.defaultProps != null)
+    if (arguments.length > 2 && (d.children = arguments.length > 3 ? d0.call(arguments, 2) : i), typeof r == "function" && r.defaultProps != null)
         for (c in r.defaultProps) d[c] === void 0 && (d[c] = r.defaultProps[c]);
-    return l0(r, d, a, l, null)
+    return c0(r, d, a, l, null)
 }
 
-function l0(r, e, i, a, l) {
+function c0(r, e, i, a, l) {
     var c = {
         type: r,
         props: e,
         key: i,
         ref: a,
         __k: null,
         __: null,
         __b: 0,
         __e: null,
         __d: void 0,
         __c: null,
         constructor: void 0,
-        __v: l ?? ++oa,
+        __v: l ?? ++ca,
         __i: -1,
         __u: 0
     };
     return l == null && Me.vnode != null && Me.vnode(c), c
 }
 
 function Ge(r) {
     return r.children
 }
 
-function c0(r, e) {
+function u0(r, e) {
     this.props = r, this.context = e
 }
 
-function er(r, e) {
-    if (e == null) return r.__ ? er(r.__, r.__i + 1) : null;
+function tr(r, e) {
+    if (e == null) return r.__ ? tr(r.__, r.__i + 1) : null;
     for (var i; e < r.__k.length; e++)
         if ((i = r.__k[e]) != null && i.__e != null) return i.__e;
-    return typeof r.type == "function" ? er(r) : null
+    return typeof r.type == "function" ? tr(r) : null
 }
 
-function ca(r) {
+function ma(r) {
     var e, i;
     if ((r = r.__) != null && r.__c != null) {
         for (r.__e = r.__c.base = null, e = 0; e < r.__k.length; e++)
             if ((i = r.__k[e]) != null && i.__e != null) {
                 r.__e = r.__c.base = i.__e;
                 break
-            } return ca(r)
+            } return ma(r)
     }
 }
 
-function ta(r) {
-    (!r.__d && (r.__d = !0) && Kt.push(r) && !u0.__r++ || ea !== Me.debounceRendering) && ((ea = Me.debounceRendering) || aa)(u0)
+function oa(r) {
+    (!r.__d && (r.__d = !0) && er.push(r) && !h0.__r++ || ia !== Me.debounceRendering) && ((ia = Me.debounceRendering) || ua)(h0)
 }
 
-function u0() {
-    var r, e, i, a, l, c, d, m, g;
-    for (Kt.sort(Mn); r = Kt.shift();) r.__d && (e = Kt.length, a = void 0, c = (l = (i = r).__v).__e, m = [], g = [], (d = i.__P) && ((a = Vt({}, l)).__v = l.__v + 1, Me.vnode && Me.vnode(a), zn(d, a, l, i.__n, d.ownerSVGElement !== void 0, 32 & l.__u ? [c] : null, m, c ?? er(l), !!(32 & l.__u), g), a.__v = l.__v, a.__.__k[a.__i] = a, da(m, a, g), a.__e != c && ca(a)), Kt.length > e && Kt.sort(Mn));
-    u0.__r = 0
+function h0() {
+    var r, e, i, a, l, c, d, f, g;
+    for (er.sort(En); r = er.shift();) r.__d && (e = er.length, a = void 0, c = (l = (i = r).__v).__e, f = [], g = [], (d = i.__P) && ((a = Vt({}, l)).__v = l.__v + 1, Me.vnode && Me.vnode(a), Rn(d, a, l, i.__n, d.ownerSVGElement !== void 0, 32 & l.__u ? [c] : null, f, c ?? tr(l), !!(32 & l.__u), g), a.__v = l.__v, a.__.__k[a.__i] = a, ga(f, a, g), a.__e != c && ma(a)), er.length > e && er.sort(En));
+    h0.__r = 0
 }
 
-function ua(r, e, i, a, l, c, d, m, g, y, _) {
-    var k, T, A, L, R, G = a && a.__k || sa,
+function pa(r, e, i, a, l, c, d, f, g, y, _) {
+    var w, T, A, L, R, O = a && a.__k || ha,
         P = e.length;
-    for (i.__d = g, hh(i, e, G), g = i.__d, k = 0; k < P; k++)(A = i.__k[k]) != null && typeof A != "boolean" && typeof A != "function" && (T = A.__i === -1 ? Tr : G[A.__i] || Tr, A.__i = k, zn(r, A, T, l, c, d, m, g, y, _), L = A.__e, A.ref && T.ref != A.ref && (T.ref && Rn(T.ref, null, A), _.push(A.ref, A.__c || L, A)), R == null && L != null && (R = L), 65536 & A.__u || T.__k === A.__k ? (L || T.__e != g || (g = er(T)), g = ha(A, g, r)) : typeof A.type == "function" && A.__d !== void 0 ? g = A.__d : L && (g = L.nextSibling), A.__d = void 0, A.__u &= -196609);
+    for (i.__d = g, dh(i, e, O), g = i.__d, w = 0; w < P; w++)(A = i.__k[w]) != null && typeof A != "boolean" && typeof A != "function" && (T = A.__i === -1 ? Tr : O[A.__i] || Tr, A.__i = w, Rn(r, A, T, l, c, d, f, g, y, _), L = A.__e, A.ref && T.ref != A.ref && (T.ref && Fn(T.ref, null, A), _.push(A.ref, A.__c || L, A)), R == null && L != null && (R = L), 65536 & A.__u || T.__k === A.__k ? (L || T.__e != g || (g = tr(T)), g = fa(A, g, r)) : typeof A.type == "function" && A.__d !== void 0 ? g = A.__d : L && (g = L.nextSibling), A.__d = void 0, A.__u &= -196609);
     i.__d = g, i.__e = R
 }
 
-function hh(r, e, i) {
-    var a, l, c, d, m, g = e.length,
+function dh(r, e, i) {
+    var a, l, c, d, f, g = e.length,
         y = i.length,
         _ = y,
-        k = 0;
-    for (r.__k = [], a = 0; a < g; a++) d = a + k, (l = r.__k[a] = (l = e[a]) == null || typeof l == "boolean" || typeof l == "function" ? null : typeof l == "string" || typeof l == "number" || typeof l == "bigint" || l.constructor == String ? l0(null, l, null, null, null) : Dn(l) ? l0(Ge, {
+        w = 0;
+    for (r.__k = [], a = 0; a < g; a++) d = a + w, (l = r.__k[a] = (l = e[a]) == null || typeof l == "boolean" || typeof l == "function" ? null : typeof l == "string" || typeof l == "number" || typeof l == "bigint" || l.constructor == String ? c0(null, l, null, null, null) : zn(l) ? c0(Ge, {
         children: l
-    }, null, null, null) : l.constructor === void 0 && l.__b > 0 ? l0(l.type, l.props, l.key, l.ref ? l.ref : null, l.__v) : l) != null ? (l.__ = r, l.__b = r.__b + 1, m = dh(l, i, d, _), l.__i = m, c = null, m !== -1 && (_--, (c = i[m]) && (c.__u |= 131072)), c == null || c.__v === null ? (m == -1 && k--, typeof l.type != "function" && (l.__u |= 65536)) : m !== d && (m === d + 1 ? k++ : m > d ? _ > g - d ? k += m - d : k-- : m < d ? m == d - 1 && (k = m - d) : k = 0, m !== a + k && (l.__u |= 65536))) : (c = i[d]) && c.key == null && c.__e && !(131072 & c.__u) && (c.__e == r.__d && (r.__d = er(c)), En(c, c, !1), i[d] = null, _--);
+    }, null, null, null) : l.constructor === void 0 && l.__b > 0 ? c0(l.type, l.props, l.key, l.ref ? l.ref : null, l.__v) : l) != null ? (l.__ = r, l.__b = r.__b + 1, f = mh(l, i, d, _), l.__i = f, c = null, f !== -1 && (_--, (c = i[f]) && (c.__u |= 131072)), c == null || c.__v === null ? (f == -1 && w--, typeof l.type != "function" && (l.__u |= 65536)) : f !== d && (f === d + 1 ? w++ : f > d ? _ > g - d ? w += f - d : w-- : f < d ? f == d - 1 && (w = f - d) : w = 0, f !== a + w && (l.__u |= 65536))) : (c = i[d]) && c.key == null && c.__e && !(131072 & c.__u) && (c.__e == r.__d && (r.__d = tr(c)), Dn(c, c, !1), i[d] = null, _--);
     if (_)
-        for (a = 0; a < y; a++)(c = i[a]) != null && !(131072 & c.__u) && (c.__e == r.__d && (r.__d = er(c)), En(c, c))
+        for (a = 0; a < y; a++)(c = i[a]) != null && !(131072 & c.__u) && (c.__e == r.__d && (r.__d = tr(c)), Dn(c, c))
 }
 
-function ha(r, e, i) {
+function fa(r, e, i) {
     var a, l;
     if (typeof r.type == "function") {
-        for (a = r.__k, l = 0; a && l < a.length; l++) a[l] && (a[l].__ = r, e = ha(a[l], e, i));
+        for (a = r.__k, l = 0; a && l < a.length; l++) a[l] && (a[l].__ = r, e = fa(a[l], e, i));
         return e
     }
     r.__e != e && (i.insertBefore(r.__e, e || null), e = r.__e);
     do e = e && e.nextSibling; while (e != null && e.nodeType === 8);
     return e
 }
 
-function dh(r, e, i, a) {
+function mh(r, e, i, a) {
     var l = r.key,
         c = r.type,
         d = i - 1,
-        m = i + 1,
+        f = i + 1,
         g = e[i];
     if (g === null || g && l == g.key && c === g.type && !(131072 & g.__u)) return i;
     if (a > (g != null && !(131072 & g.__u) ? 1 : 0))
-        for (; d >= 0 || m < e.length;) {
+        for (; d >= 0 || f < e.length;) {
             if (d >= 0) {
                 if ((g = e[d]) && !(131072 & g.__u) && l == g.key && c === g.type) return d;
                 d--
             }
-            if (m < e.length) {
-                if ((g = e[m]) && !(131072 & g.__u) && l == g.key && c === g.type) return m;
-                m++
+            if (f < e.length) {
+                if ((g = e[f]) && !(131072 & g.__u) && l == g.key && c === g.type) return f;
+                f++
             }
         }
     return -1
 }
 
-function ra(r, e, i) {
-    e[0] === "-" ? r.setProperty(e, i ?? "") : r[e] = i == null ? "" : typeof i != "number" || ch.test(e) ? i : i + "px"
+function aa(r, e, i) {
+    e[0] === "-" ? r.setProperty(e, i ?? "") : r[e] = i == null ? "" : typeof i != "number" || uh.test(e) ? i : i + "px"
 }
 
-function s0(r, e, i, a, l) {
+function l0(r, e, i, a, l) {
     var c;
     e: if (e === "style")
         if (typeof i == "string") r.style.cssText = i;
         else {
             if (typeof a == "string" && (r.style.cssText = a = ""), a)
-                for (e in a) i && e in i || ra(r.style, e, "");
+                for (e in a) i && e in i || aa(r.style, e, "");
             if (i)
-                for (e in i) a && i[e] === a[e] || ra(r.style, e, i[e])
+                for (e in i) a && i[e] === a[e] || aa(r.style, e, i[e])
         }
-    else if (e[0] === "o" && e[1] === "n") c = e !== (e = e.replace(/(PointerCapture)$|Capture$/i, "$1")), e = e.toLowerCase() in r ? e.toLowerCase().slice(2) : e.slice(2), r.l || (r.l = {}), r.l[e + c] = i, i ? a ? i.u = a.u : (i.u = Date.now(), r.addEventListener(e, c ? ia : na, c)) : r.removeEventListener(e, c ? ia : na, c);
+    else if (e[0] === "o" && e[1] === "n") c = e !== (e = e.replace(/(PointerCapture)$|Capture$/i, "$1")), e = e.toLowerCase() in r || e === "onFocusOut" || e === "onFocusIn" ? e.toLowerCase().slice(2) : e.slice(2), r.l || (r.l = {}), r.l[e + c] = i, i ? a ? i.u = a.u : (i.u = Date.now(), r.addEventListener(e, c ? la : sa, c)) : r.removeEventListener(e, c ? la : sa, c);
     else {
         if (l) e = e.replace(/xlink(H|:h)/, "h").replace(/sName$/, "s");
         else if (e !== "width" && e !== "height" && e !== "href" && e !== "list" && e !== "form" && e !== "tabIndex" && e !== "download" && e !== "rowSpan" && e !== "colSpan" && e !== "role" && e in r) try {
             r[e] = i ?? "";
             break e
         } catch {}
         typeof i == "function" || (i == null || i === !1 && e[4] !== "-" ? r.removeAttribute(e) : r.setAttribute(e, i))
     }
 }
 
-function na(r) {
+function sa(r) {
     if (this.l) {
         var e = this.l[r.type + !1];
         if (r.t) {
             if (r.t <= e.u) return
         } else r.t = Date.now();
         return e(Me.event ? Me.event(r) : r)
     }
 }
 
-function ia(r) {
+function la(r) {
     if (this.l) return this.l[r.type + !0](Me.event ? Me.event(r) : r)
 }
 
-function zn(r, e, i, a, l, c, d, m, g, y) {
-    var _, k, T, A, L, R, G, P, I, Y, re, te, j, ne, pe, ue = e.type;
+function Rn(r, e, i, a, l, c, d, f, g, y) {
+    var _, w, T, A, L, R, O, P, I, Y, re, te, j, ne, pe, ue = e.type;
     if (e.constructor !== void 0) return null;
-    128 & i.__u && (g = !!(32 & i.__u), c = [m = e.__e = i.__e]), (_ = Me.__b) && _(e);
+    128 & i.__u && (g = !!(32 & i.__u), c = [f = e.__e = i.__e]), (_ = Me.__b) && _(e);
     e: if (typeof ue == "function") try {
-        if (P = e.props, I = (_ = ue.contextType) && a[_.__c], Y = _ ? I ? I.props.value : _.__ : a, i.__c ? G = (k = e.__c = i.__c).__ = k.__E : ("prototype" in ue && ue.prototype.render ? e.__c = k = new ue(P, Y) : (e.__c = k = new c0(P, Y), k.constructor = ue, k.render = ph), I && I.sub(k), k.props = P, k.state || (k.state = {}), k.context = Y, k.__n = a, T = k.__d = !0, k.__h = [], k._sb = []), k.__s == null && (k.__s = k.state), ue.getDerivedStateFromProps != null && (k.__s == k.state && (k.__s = Vt({}, k.__s)), Vt(k.__s, ue.getDerivedStateFromProps(P, k.__s))), A = k.props, L = k.state, k.__v = e, T) ue.getDerivedStateFromProps == null && k.componentWillMount != null && k.componentWillMount(), k.componentDidMount != null && k.__h.push(k.componentDidMount);
+        if (P = e.props, I = (_ = ue.contextType) && a[_.__c], Y = _ ? I ? I.props.value : _.__ : a, i.__c ? O = (w = e.__c = i.__c).__ = w.__E : ("prototype" in ue && ue.prototype.render ? e.__c = w = new ue(P, Y) : (e.__c = w = new u0(P, Y), w.constructor = ue, w.render = fh), I && I.sub(w), w.props = P, w.state || (w.state = {}), w.context = Y, w.__n = a, T = w.__d = !0, w.__h = [], w._sb = []), w.__s == null && (w.__s = w.state), ue.getDerivedStateFromProps != null && (w.__s == w.state && (w.__s = Vt({}, w.__s)), Vt(w.__s, ue.getDerivedStateFromProps(P, w.__s))), A = w.props, L = w.state, w.__v = e, T) ue.getDerivedStateFromProps == null && w.componentWillMount != null && w.componentWillMount(), w.componentDidMount != null && w.__h.push(w.componentDidMount);
         else {
-            if (ue.getDerivedStateFromProps == null && P !== A && k.componentWillReceiveProps != null && k.componentWillReceiveProps(P, Y), !k.__e && (k.shouldComponentUpdate != null && k.shouldComponentUpdate(P, k.__s, Y) === !1 || e.__v === i.__v)) {
-                for (e.__v !== i.__v && (k.props = P, k.state = k.__s, k.__d = !1), e.__e = i.__e, e.__k = i.__k, e.__k.forEach(function(ce) {
+            if (ue.getDerivedStateFromProps == null && P !== A && w.componentWillReceiveProps != null && w.componentWillReceiveProps(P, Y), !w.__e && (w.shouldComponentUpdate != null && w.shouldComponentUpdate(P, w.__s, Y) === !1 || e.__v === i.__v)) {
+                for (e.__v !== i.__v && (w.props = P, w.state = w.__s, w.__d = !1), e.__e = i.__e, e.__k = i.__k, e.__k.forEach(function(ce) {
                         ce && (ce.__ = e)
-                    }), re = 0; re < k._sb.length; re++) k.__h.push(k._sb[re]);
-                k._sb = [], k.__h.length && d.push(k);
+                    }), re = 0; re < w._sb.length; re++) w.__h.push(w._sb[re]);
+                w._sb = [], w.__h.length && d.push(w);
                 break e
             }
-            k.componentWillUpdate != null && k.componentWillUpdate(P, k.__s, Y), k.componentDidUpdate != null && k.__h.push(function() {
-                k.componentDidUpdate(A, L, R)
+            w.componentWillUpdate != null && w.componentWillUpdate(P, w.__s, Y), w.componentDidUpdate != null && w.__h.push(function() {
+                w.componentDidUpdate(A, L, R)
             })
         }
-        if (k.context = Y, k.props = P, k.__P = r, k.__e = !1, te = Me.__r, j = 0, "prototype" in ue && ue.prototype.render) {
-            for (k.state = k.__s, k.__d = !1, te && te(e), _ = k.render(k.props, k.state, k.context), ne = 0; ne < k._sb.length; ne++) k.__h.push(k._sb[ne]);
-            k._sb = []
+        if (w.context = Y, w.props = P, w.__P = r, w.__e = !1, te = Me.__r, j = 0, "prototype" in ue && ue.prototype.render) {
+            for (w.state = w.__s, w.__d = !1, te && te(e), _ = w.render(w.props, w.state, w.context), ne = 0; ne < w._sb.length; ne++) w.__h.push(w._sb[ne]);
+            w._sb = []
         } else
-            do k.__d = !1, te && te(e), _ = k.render(k.props, k.state, k.context), k.state = k.__s; while (k.__d && ++j < 25);
-        k.state = k.__s, k.getChildContext != null && (a = Vt(Vt({}, a), k.getChildContext())), T || k.getSnapshotBeforeUpdate == null || (R = k.getSnapshotBeforeUpdate(A, L)), ua(r, Dn(pe = _ != null && _.type === Ge && _.key == null ? _.props.children : _) ? pe : [pe], e, i, a, l, c, d, m, g, y), k.base = e.__e, e.__u &= -161, k.__h.length && d.push(k), G && (k.__E = k.__ = null)
+            do w.__d = !1, te && te(e), _ = w.render(w.props, w.state, w.context), w.state = w.__s; while (w.__d && ++j < 25);
+        w.state = w.__s, w.getChildContext != null && (a = Vt(Vt({}, a), w.getChildContext())), T || w.getSnapshotBeforeUpdate == null || (R = w.getSnapshotBeforeUpdate(A, L)), pa(r, zn(pe = _ != null && _.type === Ge && _.key == null ? _.props.children : _) ? pe : [pe], e, i, a, l, c, d, f, g, y), w.base = e.__e, e.__u &= -161, w.__h.length && d.push(w), O && (w.__E = w.__ = null)
     } catch (ce) {
-        e.__v = null, g || c != null ? (e.__e = m, e.__u |= g ? 160 : 32, c[c.indexOf(m)] = null) : (e.__e = i.__e, e.__k = i.__k), Me.__e(ce, e, i)
-    } else c == null && e.__v === i.__v ? (e.__k = i.__k, e.__e = i.__e) : e.__e = mh(i.__e, e, i, a, l, c, d, g, y);
+        e.__v = null, g || c != null ? (e.__e = f, e.__u |= g ? 160 : 32, c[c.indexOf(f)] = null) : (e.__e = i.__e, e.__k = i.__k), Me.__e(ce, e, i)
+    } else c == null && e.__v === i.__v ? (e.__k = i.__k, e.__e = i.__e) : e.__e = ph(i.__e, e, i, a, l, c, d, g, y);
     (_ = Me.diffed) && _(e)
 }
 
-function da(r, e, i) {
+function ga(r, e, i) {
     e.__d = void 0;
-    for (var a = 0; a < i.length; a++) Rn(i[a], i[++a], i[++a]);
+    for (var a = 0; a < i.length; a++) Fn(i[a], i[++a], i[++a]);
     Me.__c && Me.__c(e, r), r.some(function(l) {
         try {
             r = l.__h, l.__h = [], r.some(function(c) {
                 c.call(l)
             })
         } catch (c) {
             Me.__e(c, l.__v)
         }
     })
 }
 
-function mh(r, e, i, a, l, c, d, m, g) {
-    var y, _, k, T, A, L, R, G = i.props,
+function ph(r, e, i, a, l, c, d, f, g) {
+    var y, _, w, T, A, L, R, O = i.props,
         P = e.props,
         I = e.type;
     if (I === "svg" && (l = !0), c != null) {
         for (y = 0; y < c.length; y++)
             if ((A = c[y]) && "setAttribute" in A == !!I && (I ? A.localName === I : A.nodeType === 3)) {
                 r = A, c[y] = null;
                 break
             }
     }
     if (r == null) {
         if (I === null) return document.createTextNode(P);
-        r = l ? document.createElementNS("http://www.w3.org/2000/svg", I) : document.createElement(I, P.is && P), c = null, m = !1
+        r = l ? document.createElementNS("http://www.w3.org/2000/svg", I) : document.createElement(I, P.is && P), c = null, f = !1
     }
-    if (I === null) G === P || m && r.data === P || (r.data = P);
+    if (I === null) O === P || f && r.data === P || (r.data = P);
     else {
-        if (c = c && h0.call(r.childNodes), G = i.props || Tr, !m && c != null)
-            for (G = {}, y = 0; y < r.attributes.length; y++) G[(A = r.attributes[y]).name] = A.value;
-        for (y in G) A = G[y], y == "children" || (y == "dangerouslySetInnerHTML" ? k = A : y === "key" || y in P || s0(r, y, null, A, l));
-        for (y in P) A = P[y], y == "children" ? T = A : y == "dangerouslySetInnerHTML" ? _ = A : y == "value" ? L = A : y == "checked" ? R = A : y === "key" || m && typeof A != "function" || G[y] === A || s0(r, y, A, G[y], l);
-        if (_) m || k && (_.__html === k.__html || _.__html === r.innerHTML) || (r.innerHTML = _.__html), e.__k = [];
-        else if (k && (r.innerHTML = ""), ua(r, Dn(T) ? T : [T], e, i, a, l && I !== "foreignObject", c, d, c ? c[0] : i.__k && er(i, 0), m, g), c != null)
-            for (y = c.length; y--;) c[y] != null && la(c[y]);
-        m || (y = "value", L !== void 0 && (L !== r[y] || I === "progress" && !L || I === "option" && L !== G[y]) && s0(r, y, L, G[y], !1), y = "checked", R !== void 0 && R !== r[y] && s0(r, y, R, G[y], !1))
+        if (c = c && d0.call(r.childNodes), O = i.props || Tr, !f && c != null)
+            for (O = {}, y = 0; y < r.attributes.length; y++) O[(A = r.attributes[y]).name] = A.value;
+        for (y in O) A = O[y], y == "children" || (y == "dangerouslySetInnerHTML" ? w = A : y === "key" || y in P || l0(r, y, null, A, l));
+        for (y in P) A = P[y], y == "children" ? T = A : y == "dangerouslySetInnerHTML" ? _ = A : y == "value" ? L = A : y == "checked" ? R = A : y === "key" || f && typeof A != "function" || O[y] === A || l0(r, y, A, O[y], l);
+        if (_) f || w && (_.__html === w.__html || _.__html === r.innerHTML) || (r.innerHTML = _.__html), e.__k = [];
+        else if (w && (r.innerHTML = ""), pa(r, zn(T) ? T : [T], e, i, a, l && I !== "foreignObject", c, d, c ? c[0] : i.__k && tr(i, 0), f, g), c != null)
+            for (y = c.length; y--;) c[y] != null && da(c[y]);
+        f || (y = "value", L !== void 0 && (L !== r[y] || I === "progress" && !L || I === "option" && L !== O[y]) && l0(r, y, L, O[y], !1), y = "checked", R !== void 0 && R !== r[y] && l0(r, y, R, O[y], !1))
     }
     return r
 }
 
-function Rn(r, e, i) {
+function Fn(r, e, i) {
     try {
         typeof r == "function" ? r(e) : r.current = e
     } catch (a) {
         Me.__e(a, i)
     }
 }
 
-function En(r, e, i) {
+function Dn(r, e, i) {
     var a, l;
-    if (Me.unmount && Me.unmount(r), (a = r.ref) && (a.current && a.current !== r.__e || Rn(a, null, e)), (a = r.__c) != null) {
+    if (Me.unmount && Me.unmount(r), (a = r.ref) && (a.current && a.current !== r.__e || Fn(a, null, e)), (a = r.__c) != null) {
         if (a.componentWillUnmount) try {
             a.componentWillUnmount()
         } catch (c) {
             Me.__e(c, e)
         }
         a.base = a.__P = null, r.__c = void 0
     }
     if (a = r.__k)
-        for (l = 0; l < a.length; l++) a[l] && En(a[l], e, i || typeof r.type != "function");
-    i || r.__e == null || la(r.__e), r.__ = r.__e = r.__d = void 0
+        for (l = 0; l < a.length; l++) a[l] && Dn(a[l], e, i || typeof r.type != "function");
+    i || r.__e == null || da(r.__e), r.__ = r.__e = r.__d = void 0
 }
 
-function ph(r, e, i) {
+function fh(r, e, i) {
     return this.constructor(r, i)
 }
 
-function tr(r, e, i) {
+function rr(r, e, i) {
     var a, l, c, d;
-    Me.__ && Me.__(r, e), l = (a = typeof i == "function") ? null : i && i.__k || e.__k, c = [], d = [], zn(e, r = (!a && i || e).__k = uh(Ge, null, [r]), l || Tr, Tr, e.ownerSVGElement !== void 0, !a && i ? [i] : l ? null : e.firstChild ? h0.call(e.childNodes) : null, c, !a && i ? i : l ? l.__e : e.firstChild, a, d), da(c, r, d)
+    Me.__ && Me.__(r, e), l = (a = typeof i == "function") ? null : i && i.__k || e.__k, c = [], d = [], Rn(e, r = (!a && i || e).__k = hh(Ge, null, [r]), l || Tr, Tr, e.ownerSVGElement !== void 0, !a && i ? [i] : l ? null : e.firstChild ? d0.call(e.childNodes) : null, c, !a && i ? i : l ? l.__e : e.firstChild, a, d), ga(c, r, d)
 }
-h0 = sa.slice, Me = {
+d0 = ha.slice, Me = {
     __e: function(r, e, i, a) {
         for (var l, c, d; e = e.__;)
             if ((l = e.__c) && !l.__) try {
                 if ((c = l.constructor) && c.getDerivedStateFromError != null && (l.setState(c.getDerivedStateFromError(r)), d = l.__d), l.componentDidCatch != null && (l.componentDidCatch(r, a || {}), d = l.__d), d) return l.__E = l
-            } catch (m) {
-                r = m
+            } catch (f) {
+                r = f
             }
         throw r
     }
-}, oa = 0, sh = function(r) {
+}, ca = 0, lh = function(r) {
     return r != null && r.constructor == null
-}, c0.prototype.setState = function(r, e) {
+}, u0.prototype.setState = function(r, e) {
     var i;
-    i = this.__s != null && this.__s !== this.state ? this.__s : this.__s = Vt({}, this.state), typeof r == "function" && (r = r(Vt({}, i), this.props)), r && Vt(i, r), r != null && this.__v && (e && this._sb.push(e), ta(this))
-}, c0.prototype.forceUpdate = function(r) {
-    this.__v && (this.__e = !0, r && this.__h.push(r), ta(this))
-}, c0.prototype.render = Ge, Kt = [], aa = typeof Promise == "function" ? Promise.prototype.then.bind(Promise.resolve()) : setTimeout, Mn = function(r, e) {
+    i = this.__s != null && this.__s !== this.state ? this.__s : this.__s = Vt({}, this.state), typeof r == "function" && (r = r(Vt({}, i), this.props)), r && Vt(i, r), r != null && this.__v && (e && this._sb.push(e), oa(this))
+}, u0.prototype.forceUpdate = function(r) {
+    this.__v && (this.__e = !0, r && this.__h.push(r), oa(this))
+}, u0.prototype.render = Ge, er = [], ua = typeof Promise == "function" ? Promise.prototype.then.bind(Promise.resolve()) : setTimeout, En = function(r, e) {
     return r.__v.__b - e.__v.__b
-}, u0.__r = 0, lh = 0;
+}, h0.__r = 0, ch = 0;
 
 function jt(r, e) {
     if (e == null || r.frontierEntries == null || r.frontierEntries.length === 0) return r;
     {
         (e < 0 || e >= r.frontierEntries.length) && (e = 0);
         let i = r.frontierEntries[e];
         return {
@@ -16342,322 +16347,322 @@
             logicalQubit: i.logicalQubit,
             tfactory: i.tfactory,
             errorBudget: i.errorBudget,
             logicalCounts: r.logicalCounts
         }
     }
 }
-var Ar, Ue, Fn, ma, p0 = 0,
-    wa = [],
-    d0 = [],
+var Ar, Ue, Bn, ba, f0 = 0,
+    Ca = [],
+    m0 = [],
     Ye = Me,
-    pa = Ye.__b,
-    fa = Ye.__r,
-    ga = Ye.diffed,
-    ba = Ye.__c,
-    ya = Ye.unmount,
-    xa = Ye.__;
+    ya = Ye.__b,
+    xa = Ye.__r,
+    va = Ye.diffed,
+    wa = Ye.__c,
+    ka = Ye.unmount,
+    _a = Ye.__;
 
-function Nn(r, e) {
-    Ye.__h && Ye.__h(Ue, r, p0 || e), p0 = 0;
+function Ln(r, e) {
+    Ye.__h && Ye.__h(Ue, r, f0 || e), f0 = 0;
     var i = Ue.__H || (Ue.__H = {
         __: [],
         __h: []
     });
     return r >= i.__.length && i.__.push({
-        __V: d0
+        __V: m0
     }), i.__[r]
 }
 
-function Ke(r) {
-    return p0 = 1, fh(_a, r)
+function Xe(r) {
+    return f0 = 1, gh(Aa, r)
 }
 
-function fh(r, e, i) {
-    var a = Nn(Ar++, 2);
-    if (a.t = r, !a.__c && (a.__ = [i ? i(e) : _a(void 0, e), function(m) {
+function gh(r, e, i) {
+    var a = Ln(Ar++, 2);
+    if (a.t = r, !a.__c && (a.__ = [i ? i(e) : Aa(void 0, e), function(f) {
             var g = a.__N ? a.__N[0] : a.__[0],
-                y = a.t(g, m);
+                y = a.t(g, f);
             g !== y && (a.__N = [y, a.__[1]], a.__c.setState({}))
         }], a.__c = Ue, !Ue.u)) {
-        var l = function(m, g, y) {
+        var l = function(f, g, y) {
             if (!a.__c.__H) return !0;
             var _ = a.__c.__H.__.filter(function(T) {
                 return !!T.__c
             });
             if (_.every(function(T) {
                     return !T.__N
-                })) return !c || c.call(this, m, g, y);
-            var k = !1;
+                })) return !c || c.call(this, f, g, y);
+            var w = !1;
             return _.forEach(function(T) {
                 if (T.__N) {
                     var A = T.__[0];
-                    T.__ = T.__N, T.__N = void 0, A !== T.__[0] && (k = !0)
+                    T.__ = T.__N, T.__N = void 0, A !== T.__[0] && (w = !0)
                 }
-            }), !(!k && a.__c.props === m) && (!c || c.call(this, m, g, y))
+            }), !(!w && a.__c.props === f) && (!c || c.call(this, f, g, y))
         };
         Ue.u = !0;
         var c = Ue.shouldComponentUpdate,
             d = Ue.componentWillUpdate;
-        Ue.componentWillUpdate = function(m, g, y) {
+        Ue.componentWillUpdate = function(f, g, y) {
             if (this.__e) {
                 var _ = c;
-                c = void 0, l(m, g, y), c = _
+                c = void 0, l(f, g, y), c = _
             }
-            d && d.call(this, m, g, y)
+            d && d.call(this, f, g, y)
         }, Ue.shouldComponentUpdate = l
     }
     return a.__N || a.__
 }
 
-function cr(r, e) {
-    var i = Nn(Ar++, 3);
-    !Ye.__s && ka(i.__H, e) && (i.__ = r, i.i = e, Ue.__H.__h.push(i))
+function Ut(r, e) {
+    var i = Ln(Ar++, 3);
+    !Ye.__s && Ta(i.__H, e) && (i.__ = r, i.i = e, Ue.__H.__h.push(i))
 }
 
 function St(r) {
-    return p0 = 5, gh(function() {
+    return f0 = 5, bh(function() {
         return {
             current: r
         }
     }, [])
 }
 
-function gh(r, e) {
-    var i = Nn(Ar++, 7);
-    return ka(i.__H, e) ? (i.__V = r(), i.i = e, i.__h = r, i.__V) : i.__
+function bh(r, e) {
+    var i = Ln(Ar++, 7);
+    return Ta(i.__H, e) ? (i.__V = r(), i.i = e, i.__h = r, i.__V) : i.__
 }
 
-function bh() {
-    for (var r; r = wa.shift();)
+function yh() {
+    for (var r; r = Ca.shift();)
         if (r.__P && r.__H) try {
-            r.__H.__h.forEach(m0), r.__H.__h.forEach(Bn), r.__H.__h = []
+            r.__H.__h.forEach(p0), r.__H.__h.forEach(Nn), r.__H.__h = []
         } catch (e) {
             r.__H.__h = [], Ye.__e(e, r.__v)
         }
 }
 Ye.__b = function(r) {
-    Ue = null, pa && pa(r)
+    Ue = null, ya && ya(r)
 }, Ye.__ = function(r, e) {
-    r && e.__k && e.__k.__m && (r.__m = e.__k.__m), xa && xa(r, e)
+    r && e.__k && e.__k.__m && (r.__m = e.__k.__m), _a && _a(r, e)
 }, Ye.__r = function(r) {
-    fa && fa(r), Ar = 0;
+    xa && xa(r), Ar = 0;
     var e = (Ue = r.__c).__H;
-    e && (Fn === Ue ? (e.__h = [], Ue.__h = [], e.__.forEach(function(i) {
-        i.__N && (i.__ = i.__N), i.__V = d0, i.__N = i.i = void 0
-    })) : (e.__h.forEach(m0), e.__h.forEach(Bn), e.__h = [], Ar = 0)), Fn = Ue
+    e && (Bn === Ue ? (e.__h = [], Ue.__h = [], e.__.forEach(function(i) {
+        i.__N && (i.__ = i.__N), i.__V = m0, i.__N = i.i = void 0
+    })) : (e.__h.forEach(p0), e.__h.forEach(Nn), e.__h = [], Ar = 0)), Bn = Ue
 }, Ye.diffed = function(r) {
-    ga && ga(r);
+    va && va(r);
     var e = r.__c;
-    e && e.__H && (e.__H.__h.length && (wa.push(e) !== 1 && ma === Ye.requestAnimationFrame || ((ma = Ye.requestAnimationFrame) || yh)(bh)), e.__H.__.forEach(function(i) {
-        i.i && (i.__H = i.i), i.__V !== d0 && (i.__ = i.__V), i.i = void 0, i.__V = d0
-    })), Fn = Ue = null
+    e && e.__H && (e.__H.__h.length && (Ca.push(e) !== 1 && ba === Ye.requestAnimationFrame || ((ba = Ye.requestAnimationFrame) || xh)(yh)), e.__H.__.forEach(function(i) {
+        i.i && (i.__H = i.i), i.__V !== m0 && (i.__ = i.__V), i.i = void 0, i.__V = m0
+    })), Bn = Ue = null
 }, Ye.__c = function(r, e) {
     e.some(function(i) {
         try {
-            i.__h.forEach(m0), i.__h = i.__h.filter(function(a) {
-                return !a.__ || Bn(a)
+            i.__h.forEach(p0), i.__h = i.__h.filter(function(a) {
+                return !a.__ || Nn(a)
             })
         } catch (a) {
             e.some(function(l) {
                 l.__h && (l.__h = [])
             }), e = [], Ye.__e(a, i.__v)
         }
-    }), ba && ba(r, e)
+    }), wa && wa(r, e)
 }, Ye.unmount = function(r) {
-    ya && ya(r);
+    ka && ka(r);
     var e, i = r.__c;
     i && i.__H && (i.__H.__.forEach(function(a) {
         try {
-            m0(a)
+            p0(a)
         } catch (l) {
             e = l
         }
     }), i.__H = void 0, e && Ye.__e(e, i.__v))
 };
-var va = typeof requestAnimationFrame == "function";
+var Sa = typeof requestAnimationFrame == "function";
 
-function yh(r) {
+function xh(r) {
     var e, i = function() {
-            clearTimeout(a), va && cancelAnimationFrame(e), setTimeout(r)
+            clearTimeout(a), Sa && cancelAnimationFrame(e), setTimeout(r)
         },
         a = setTimeout(i, 100);
-    va && (e = requestAnimationFrame(i))
+    Sa && (e = requestAnimationFrame(i))
 }
 
-function m0(r) {
+function p0(r) {
     var e = Ue,
         i = r.__c;
     typeof i == "function" && (r.__c = void 0, i()), Ue = e
 }
 
-function Bn(r) {
+function Nn(r) {
     var e = Ue;
     r.__c = r.__(), Ue = e
 }
 
-function ka(r, e) {
+function Ta(r, e) {
     return !r || r.length !== e.length || e.some(function(i, a) {
         return i !== r[a]
     })
 }
 
-function _a(r, e) {
+function Aa(r, e) {
     return typeof e == "function" ? e(r) : e
 }
-var xh = 0,
-    pf = Array.isArray;
+var vh = 0,
+    vf = Array.isArray;
 
 function M(r, e, i, a, l, c) {
-    var d, m, g = {};
-    for (m in e) m == "ref" ? d = e[m] : g[m] = e[m];
+    var d, f, g = {};
+    for (f in e) f == "ref" ? d = e[f] : g[f] = e[f];
     var y = {
         type: r,
         props: g,
         key: i,
         ref: d,
         __k: null,
         __: null,
         __b: 0,
         __e: null,
         __d: void 0,
         __c: null,
         constructor: void 0,
-        __v: --xh,
+        __v: --vh,
         __i: -1,
         __u: 0,
         __source: l,
         __self: c
     };
     if (typeof r == "function" && (d = r.defaultProps))
-        for (m in d) g[m] === void 0 && (g[m] = d[m]);
+        for (f in d) g[f] === void 0 && (g[f] = d[f]);
     return Me.vnode && Me.vnode(y), y
 }
-var Sa = !1,
-    Ca = !0,
-    f0 = [{
+var qa = !1,
+    Ma = !0,
+    g0 = [{
         category: "itemCount",
         options: ["Show all", "Top 10", "Top 25"]
     }, {
         category: "sortOrder",
         options: ["Sort a-z", "High to low", "Low to high"]
     }, {
         category: "labels",
         options: ["Raw labels", "Ket labels", "No labels"]
     }],
-    Ta = 3,
-    vh = {
+    Ea = 3,
+    wh = {
         itemCount: 0,
         sortOrder: 0,
         labels: 0
     },
-    wh = /^\[(?:(Zero|One), *)*(Zero|One)\]$/;
+    kh = /^\[(?:(Zero|One), *)*(Zero|One)\]$/;
 
-function Aa(r) {
+function Da(r) {
     if (typeof r != "string") return "ERROR";
-    if (wh.test(r)) {
+    if (kh.test(r)) {
         let e = r.match(/(One|Zero)/g),
             i = "|";
         return e?.forEach(a => i += a == "One" ? "1" : "0"), i += "\u27E9", i
     } else return r
 }
 
-function Ln(r) {
-    let [e, i] = Ke(""), [a, l] = Ke({
+function Pn(r) {
+    let [e, i] = Xe(""), [a, l] = Xe({
         zoom: 1,
         offset: 1
-    }), [c, d] = Ke(vh), m = St(null), g = St(null), y = 0;
+    }), [c, d] = Xe(wh), f = St(null), g = St(null), y = 0;
     switch (c.itemCount) {
         case 1:
             y = 10;
             break;
         case 2:
             y = 25;
             break
     }
     let _ = c.labels === 1,
-        k = [...r.data],
+        w = [...r.data],
         T = 0,
         A = 0;
-    k.forEach(ee => {
+    w.forEach(ee => {
         T += ee[1], A = Math.max(ee[1], A)
     });
-    let L = `${k.length} unique results`;
-    y > 0 && (k.sort((ee, $) => ee[1] < $[1] ? 1 : -1), k.length > y && (L = `Top ${y} of ${L}`, k.length = y)), r.filter && (L += `. Shot filter: ${_?Aa(r.filter):r.filter}`), k.sort((ee, $) => {
+    let L = `${w.length} unique results`;
+    y > 0 && (w.sort((ee, G) => ee[1] < G[1] ? 1 : -1), w.length > y && (L = `Top ${y} of ${L}`, w.length = y)), r.filter && (L += `. Shot filter: ${_?Da(r.filter):r.filter}`), w.sort((ee, G) => {
         let fe = Number(ee[0]),
-            Te = Number($[0]);
+            Te = Number(G[0]);
         switch (c.sortOrder) {
             case 1:
-                return ee[1] < $[1] ? 1 : -1;
+                return ee[1] < G[1] ? 1 : -1;
             case 2:
-                return ee[1] > $[1] ? 1 : -1;
+                return ee[1] > G[1] ? 1 : -1;
             default:
-                return !isNaN(fe) && !isNaN(Te) ? fe < Te ? -1 : 1 : ee[0] < $[0] ? -1 : 1
+                return !isNaN(fe) && !isNaN(Te) ? fe < Te ? -1 : 1 : ee[0] < G[0] ? -1 : 1
         }
     });
 
     function R(ee) {
         let fe = ee.target.querySelector("title")?.textContent;
         i(fe || "")
     }
 
-    function G() {
+    function O() {
         i("")
     }
 
     function P(ee) {
         let fe = ee.target.getAttribute("data-raw-label");
         fe === r.filter ? r.onFilter("") : r.onFilter(fe || "")
     }
 
     function I() {
-        m.current && (m.current.style.display === "inline" ? m.current.style.display = "none" : (m.current.style.display = "inline", g.current && (g.current.style.display = "none")))
+        f.current && (f.current.style.display === "inline" ? f.current.style.display = "none" : (f.current.style.display = "inline", g.current && (g.current.style.display = "none")))
     }
 
-    function Y(ee, $) {
-        if (!m.current) return;
+    function Y(ee, G) {
+        if (!f.current) return;
         let fe = {
             ...c
         };
-        fe[ee] = $, d(fe), ee === "itemCount" && l({
+        fe[ee] = G, d(fe), ee === "itemCount" && l({
             zoom: 1,
             offset: 1
-        }), m.current.style.display = "none"
+        }), f.current.style.display = "none"
     }
 
     function re() {
         g.current && (g.current.style.display === "inline" ? g.current.style.display = "none" : g.current.style.display = "inline")
     }
     let te = 38,
         j = 11,
-        ne = f0.length * te - 2,
-        pe = Ta * j + 3,
+        ne = g0.length * te - 2,
+        pe = Ea * j + 3,
         ue = 163,
         ce = 72,
         Ce = 1.2,
-        De = ue * a.zoom / k.length,
+        De = ue * a.zoom / w.length,
         X = De * .1,
         he = De - 2 * X,
         oe = De > 5 && c.labels !== 2;
 
     function ae(ee) {
         ee.preventDefault();
-        let $ = ee.currentTarget,
-            fe = new DOMPoint(ee.clientX, ee.clientY).matrixTransform($.getScreenCTM()?.inverse()),
+        let G = ee.currentTarget,
+            fe = new DOMPoint(ee.clientX, ee.clientY).matrixTransform(G.getScreenCTM()?.inverse()),
             Te = a.offset,
             Ae = a.zoom;
-        if (!Ca || !ee.altKey) {
+        if (!Ma || !ee.altKey) {
             Ae = a.zoom + ee.deltaY * .05, Ae = Math.min(Math.max(1, Ae), 50);
             let Pt = ue * a.zoom,
-                O0 = (0 - a.offset + fe.x) / Pt,
-                H0 = Ae * ue - a.zoom * ue,
-                $0 = O0 * H0;
-            Te = a.offset - $0
+                H0 = (0 - a.offset + fe.x) / Pt,
+                $0 = Ae * ue - a.zoom * ue,
+                G0 = H0 * $0;
+            Te = a.offset - G0
         }
-        Sa && (Te -= ee.deltaX), !Sa && Ca && ee.altKey && (Te -= ee.deltaY);
+        qa && (Te -= ee.deltaX), !qa && Ma && ee.altKey && (Te -= ee.deltaY);
         let qt = 1 - (ue * Ae - ue),
             ct = Math.min(Math.max(Te, qt), 1);
         l({
             zoom: Ae,
             offset: ct
         })
     }
@@ -16667,31 +16672,31 @@
             children: ["Total shots: ", r.shotCount]
         }) : null, M("svg", {
             class: "histogram",
             viewBox: "0 0 165 100",
             onWheel: ae,
             children: [M("g", {
                 transform: `translate(${a.offset},4)`,
-                children: k.map((ee, $) => {
-                    let fe = _ ? Aa(ee[0]) : ee[0],
+                children: w.map((ee, G) => {
+                    let fe = _ ? Da(ee[0]) : ee[0],
                         Te = ce * (ee[1] / A),
-                        Ae = De * $ + X,
-                        qt = De * $ + De / 2 - Ce,
+                        Ae = De * G + X,
+                        qt = De * G + De / 2 - Ce,
                         ct = ce + 15 - Te,
                         Pt = `${fe} at ${(ee[1]/T*100).toFixed(2)}%`,
                         yr = "bar";
                     return ee[0] === r.filter && (yr += " bar-selected"), M(Ge, {
                         children: [M("rect", {
                             class: yr,
                             x: Ae,
                             y: ct,
                             width: he,
                             height: Te,
                             onMouseOver: R,
-                            onMouseOut: G,
+                            onMouseOut: O,
                             onClick: P,
                             "data-raw-label": ee[0],
                             children: M("title", {
                                 children: Pt
                             })
                         }), M("text", {
                             class: "bar-label",
@@ -16764,46 +16769,46 @@
                 }), M("path", {
                     "stroke-width": "2.5",
                     "stroke-linecap": "round",
                     d: "M12 8 V8 M12 12.5 V18"
                 })]
             }), M("g", {
                 id: "menu",
-                ref: m,
+                ref: f,
                 transform: "translate(8, 2)",
                 style: "display: none;",
                 children: [M("rect", {
                     x: "0",
                     y: "0",
                     rx: "2",
                     width: ne,
                     height: pe,
                     class: "menu-box"
-                }), f0.map((ee, $) => ee.options.map((fe, Te) => {
+                }), g0.map((ee, G) => ee.options.map((fe, Te) => {
                     let Ae = "menu-item";
                     return c[ee.category] === Te && (Ae += " menu-selected"), M(Ge, {
                         children: [M("rect", {
-                            x: 2 + $ * te,
+                            x: 2 + G * te,
                             y: 2 + Te * j,
                             rx: "1",
                             class: Ae,
                             onClick: () => Y(ee.category, Te)
                         }), M("text", {
-                            x: 5 + $ * te,
+                            x: 5 + G * te,
                             y: 9 + Te * j,
                             class: "menu-text",
                             children: fe
                         })]
                     })
-                })), f0.map((ee, $) => $ >= f0.length - 1 ? null : M("line", {
+                })), g0.map((ee, G) => G >= g0.length - 1 ? null : M("line", {
                     class: "menu-separator",
-                    x1: 37 + $ * te,
+                    x1: 37 + G * te,
                     y1: "2",
-                    x2: 37 + $ * te,
-                    y2: Ta * j + 1
+                    x2: 37 + G * te,
+                    y2: Ea * j + 1
                 }))]
             }), M("g", {
                 ref: g,
                 style: "display: none;",
                 children: [M("rect", {
                     width: "155",
                     height: "76",
@@ -16846,15 +16851,15 @@
                     })]
                 })]
             })]
         })]
     })
 }
 
-function qa(r) {
+function za(r) {
     let e = [],
         i = [],
         a = new Intl.NumberFormat,
         l = new Intl.NumberFormat(void 0, {
             maximumFractionDigits: 2,
             minimumFractionDigits: 2
         });
@@ -17203,17 +17208,17 @@
     }), {
         groups: e,
         assumptions: ["_More details on the following lists of assumptions can be found in the paper [Accessing requirements for scaling quantum computers and their applications](https://aka.ms/AQ/RE/Paper)._", "**Uniform independent physical noise.** We assume that the noise on physical qubits and physical qubit operations is the standard circuit noise model. In particular we assume error events at different space-time locations are independent and that error rates are uniform across the system in time and space.", "**Efficient classical computation.** We assume that classical overhead (compilation, control, feedback, readout, decoding, etc.) does not dominate the overall cost of implementing the full quantum algorithm.", "**Extraction circuits for planar quantum ISA.** We assume that stabilizer extraction circuits with similar depth and error correction performance to those for standard surface and Hastings-Haah code patches can be constructed to implement all operations of the planar quantum ISA (instruction set architecture).", "**Uniform independent logical noise.** We assume that the error rate of a logical operation is approximately equal to its space-time volume (the number of tiles multiplied by the number of logical time steps) multiplied by the error rate of a logical qubit in a standard one-tile patch in one logical time step.", "**Negligible Clifford costs for synthesis.** We assume that the space overhead for synthesis and space and time overhead for transport of magic states within magic state factories and to synthesis qubits are all negligible.", "**Smooth magic state consumption rate.** We assume that the rate of T state consumption throughout the compiled algorithm is almost constant, or can be made almost constant without significantly increasing the number of logical time steps for the algorithm."]
     }
 }
 
 function qr(r) {
-    let [e, i] = Ke(!1), a = () => {
+    let [e, i] = Xe(!1), a = () => {
         i(!e)
-    }, l = qa(r.estimatesData);
+    }, l = za(r.estimatesData);
     return M("div", {
         children: [M("div", {
             children: [M("input", {
                 type: "checkbox",
                 id: "showDetail",
                 checked: e,
                 onClick: a
@@ -17226,15 +17231,15 @@
             children: [M("summary", {
                 children: M("strong", {
                     children: c.title
                 })
             }), M("table", {
                 className: "estimate-table",
                 children: c.entries.map(d => {
-                    let g = d.path.split("/").reduce((_, k) => _[k], r.estimatesData);
+                    let g = d.path.split("/").reduce((_, w) => _[w], r.estimatesData);
                     typeof g == "object" && (g = JSON.stringify(g));
                     let y = {
                         __html: r.mdRenderer(d.explanation)
                     };
                     return M("tr", {
                         children: [M("td", {
                             className: "estimate-cell title-cell",
@@ -17275,49 +17280,49 @@
                     }
                 }))
             })]
         })]
     })
 }
 
-function Ma(r, e, i, a, l, c) {
+function Ra(r, e, i, a, l, c) {
     let d = l - a <= 180 ? "0" : "1",
-        m = r + i * Math.cos(Math.PI * a / 180),
+        f = r + i * Math.cos(Math.PI * a / 180),
         g = e + i * Math.sin(Math.PI * a / 180),
         y = r + i * Math.cos(Math.PI * l / 180),
         _ = e + i * Math.sin(Math.PI * l / 180),
-        k = r + c * Math.cos(Math.PI * a / 180),
+        w = r + c * Math.cos(Math.PI * a / 180),
         T = e + c * Math.sin(Math.PI * a / 180),
         A = r + c * Math.cos(Math.PI * l / 180),
         L = e + c * Math.sin(Math.PI * l / 180);
-    return `M ${m} ${g} A ${i} ${i} 0 ${d} 1 ${y} ${_} L ${A} ${L} A ${c} ${c} 0 ${d} 0 ${k} ${T} Z`
+    return `M ${f} ${g} A ${i} ${i} 0 ${d} 1 ${y} ${_} L ${A} ${L} A ${c} ${c} 0 ${d} 0 ${w} ${T} Z`
 }
 
 function Mr(r) {
     let e = r.estimatesData.physicalCounts.breakdown,
         i = e.physicalQubitsForAlgorithm,
         a = e.physicalQubitsForTfactories,
         c = 360 * (i / (i + a)),
         d = c >= 360 ? 359.9 : c <= 0 ? .1 : c,
-        m = e.numTfactories,
-        g = Math.round(a / m);
+        f = e.numTfactories,
+        g = Math.round(a / f);
     return M("div", {
         style: "display: flex; flex-wrap: wrap; margin-top: 8px;",
         children: [M("svg", {
             class: "qs-widget-spaceChart",
             width: "400",
             height: "400",
             viewBox: "50 0 450 450",
             id: "pieChart",
             children: [M("path", {
-                d: Ma(250, 185, 180, 0, d, 120),
+                d: Ra(250, 185, 180, 0, d, 120),
                 fill: "var(--vscode-charts-orange, orange)",
                 stroke: "white"
             }), M("path", {
-                d: Ma(250, 185, 180, d, 360, 120),
+                d: Ra(250, 185, 180, d, 360, 120),
                 fill: "var(--vscode-charts-blue, blue)",
                 stroke: "white"
             }), M("text", {
                 x: "250",
                 y: "180",
                 "text-anchor": "middle",
                 "font-size": "16",
@@ -17440,39 +17445,39 @@
                     children: r.estimatesData.logicalQubit.physicalQubits.toLocaleString()
                 })]
             })]
         })]
     })
 }
 
-function Ea(r, e) {
+function Fa(r, e) {
     if (e < r || r <= 0) return [];
     let i = new Intl.NumberFormat,
         a = Math.round(10 ** Math.floor(Math.log10(r))),
         l = Math.round(10 ** Math.ceil(Math.log10(e))),
         c = [];
     for (let d = a; d <= l; d *= 10) d >= r && d <= e && c.push({
         value: d,
         label: i.format(d)
     });
     if (c.length == 0) {
         let d = a;
         for (; d >= 1;) {
-            let m = Math.ceil(r / d) * d;
-            for (; m <= e;) c.push({
-                value: m,
-                label: i.format(m)
-            }), m += d;
+            let f = Math.ceil(r / d) * d;
+            for (; f <= e;) c.push({
+                value: f,
+                label: i.format(f)
+            }), f += d;
             if (c.length > 0) break;
             d /= 10
         }
     }
     return c
 }
-var Xe = [{
+var Je = [{
     tick: {
         value: 1,
         label: "1 nanosecond"
     },
     plural: "nanoseconds"
 }, {
     tick: {
@@ -17538,142 +17543,142 @@
     tick: {
         value: 31536e14,
         label: "1 century"
     },
     plural: "centuries"
 }];
 
-function Da(r, e) {
+function Ba(r, e) {
     if (e < r || r <= 0) return [];
     let i = 0;
-    for (; i < Xe.length && Xe[i].tick.value <= r;) i++;
+    for (; i < Je.length && Je[i].tick.value <= r;) i++;
     let a = i;
-    for (i > 0 && i--, a >= Xe.length && (a = Xe.length - 1); a < Xe.length - 1 && Xe[a].tick.value <= e;) a++;
+    for (i > 0 && i--, a >= Je.length && (a = Je.length - 1); a < Je.length - 1 && Je[a].tick.value <= e;) a++;
     let l = [];
-    for (let c = i; c <= a; c++) Xe[c].tick.value >= r && Xe[c].tick.value <= e && l.push(Xe[c].tick);
+    for (let c = i; c <= a; c++) Je[c].tick.value >= r && Je[c].tick.value <= e && l.push(Je[c].tick);
     if (l.length == 0)
-        if (i < Xe.length - 1) {
-            let c = 10 ** Math.floor(Math.log10(Xe[i + 1].tick.value / Xe[i].tick.value));
+        if (i < Je.length - 1) {
+            let c = 10 ** Math.floor(Math.log10(Je[i + 1].tick.value / Je[i].tick.value));
             do {
                 let d = 1,
-                    m = 0;
-                do m = Xe[i].tick.value * d * c, m >= r && m <= e && l.push({
-                    value: m,
-                    label: (d * c).toString() + " " + Xe[i].plural
-                }), d++; while ((d > 2 || l.length < 1) && m < Xe[i + 1].tick.value);
+                    f = 0;
+                do f = Je[i].tick.value * d * c, f >= r && f <= e && l.push({
+                    value: f,
+                    label: (d * c).toString() + " " + Je[i].plural
+                }), d++; while ((d > 2 || l.length < 1) && f < Je[i + 1].tick.value);
                 c /= 10
             } while (l.length < 1 && c >= 1)
         } else {
-            let c = Xe.length - 1;
+            let c = Je.length - 1;
             do {
-                let d = 10 ** Math.floor(Math.log10(e / Xe[c].tick.value));
+                let d = 10 ** Math.floor(Math.log10(e / Je[c].tick.value));
                 do {
-                    let m = 1,
+                    let f = 1,
                         g = 0;
-                    do g = Xe[c].tick.value * m * d, g >= r && g <= e && l.push({
+                    do g = Je[c].tick.value * f * d, g >= r && g <= e && l.push({
                         value: g,
-                        label: (m * d).toString() + " " + Xe[c].plural
-                    }), m++; while ((m > 2 || l.length < 1) && g < e);
+                        label: (f * d).toString() + " " + Je[c].plural
+                    }), f++; while ((f > 2 || l.length < 1) && g < e);
                     d /= 10
                 } while (l.length < 1 && d >= 1);
                 c--
             } while (l.length < 1 && c >= 0)
         } return l
 }
 
-function kh(r) {
+function _h(r) {
     return r.reduce((e, i) => i.items.reduce((a, l) => [Math.min(a[0], l.x), Math.max(a[1], l.x), Math.min(a[2], l.y), Math.max(a[3], l.y)], e), [Number.MAX_VALUE, Number.MIN_VALUE, Number.MAX_VALUE, Number.MIN_VALUE])
 }
 
-function za(r, e) {
-    let [i, a, l, c] = kh(r), d = {
+function Na(r, e) {
+    let [i, a, l, c] = _h(r), d = {
         min: i / e,
         max: a * e
-    }, m = {
+    }, f = {
         min: l / e,
         max: c * e
     };
     return {
         rangeX: d,
-        rangeY: m
+        rangeY: f
     }
 }
 
-function Pn(r) {
+function In(r) {
     let e = St(null),
         {
             rangeX: i,
             rangeY: a
-        } = za(r.data, 2);
+        } = Na(r.data, 2);
 
     function l(ae, ee) {
-        return ee ? Da(ae.min, ae.max) : Ea(ae.min, ae.max)
+        return ee ? Ba(ae.min, ae.max) : Fa(ae.min, ae.max)
     }
     let c = l(i, r.xAxis.isTime),
         d = l(a, r.yAxis.isTime);
 
-    function m(ae, ee) {
+    function f(ae, ee) {
         return (Math.log(ae) - Math.log(ee.min)) / (Math.log(ee.max) - Math.log(ee.min))
     }
 
     function g(ae) {
-        return m(ae, i) * pe
+        return f(ae, i) * pe
     }
 
     function y(ae) {
-        return -m(ae, a) * ue
+        return -f(ae, a) * ue
     }
     let _ = 20,
-        k = 100,
+        w = 100,
         T = 5,
         A = 1,
-        L = _ + k + T + A,
+        L = _ + w + T + A,
         R = 160,
-        G = 20,
+        O = 20,
         P = 16,
-        I = G + P + T + A,
+        I = O + P + T + A,
         Y = 960,
         re = 50,
         te = 480,
         j = 10,
         ne = -L,
         pe = Y - L - R,
         ue = te - I,
         ce = `${ne} ${-ue-j} ${Y+re} ${te+j}`,
         Ce = 5,
         De = 4;
 
-    function U(ae, ee, $) {
+    function U(ae, ee, G) {
         let fe = ee.getAttribute("data-label");
-        $.textContent = fe;
-        let Te = $.offsetWidth / 2,
+        G.textContent = fe;
+        let Te = G.offsetWidth / 2,
             Ae = ee.getBoundingClientRect(),
             qt = (Ae.top + Ae.bottom) / 2,
             ct = (Ae.left + Ae.right) / 2,
             Pt = ae.getBoundingClientRect();
-        $.style.left = `${ct-Pt.left-Te}px`, $.style.top = `${qt-Pt.top+12}px`, $.style.visibility = "visible"
+        G.style.left = `${ct-Pt.left-Te}px`, G.style.top = `${qt-Pt.top+12}px`, G.style.visibility = "visible"
     }
 
     function X(ae, ee) {
         if (!(ae.target instanceof SVGCircleElement)) return;
-        let $ = ae.target;
-        if (!$.classList.contains("qs-scatterChart-point")) return;
-        let fe = $.closest("div"),
+        let G = ae.target;
+        if (!G.classList.contains("qs-scatterChart-point")) return;
+        let fe = G.closest("div"),
             Te = fe.querySelector(".qs-scatterChart-tooltip");
         switch (ee) {
             case "over":
-                U(fe, $, Te);
+                U(fe, G, Te);
                 break;
             case "out":
                 Te.style.visibility = "hidden";
                 break;
             case "click":
-                if ($.classList.contains("qs-scatterChart-point-selected")) r.onPointSelected(-1, 0);
+                if (G.classList.contains("qs-scatterChart-point-selected")) r.onPointSelected(-1, 0);
                 else {
-                    let Ae = JSON.parse($.getAttribute("data-index"));
+                    let Ae = JSON.parse(G.getAttribute("data-index"));
                     r.onPointSelected(Ae[0], Ae[1])
                 }
                 break;
             default:
                 console.error("Unknown event type: ", ee)
         }
     }
@@ -17683,15 +17688,15 @@
         let ae = r.data[r.selectedPoint[0]];
         return {
             ...ae.items[r.selectedPoint[1]],
             color: ae.color
         }
     }
     let oe = he();
-    return cr(() => {
+    return Ut(() => {
         if (e.current)
             if (!r.selectedPoint) e.current.style.visibility = "hidden";
             else {
                 let ae = e.current.parentElement,
                     ee = ae?.querySelector(".qs-scatterChart-point-selected");
                 if (!ee) return;
                 U(ae, ee, e.current)
@@ -17746,37 +17751,37 @@
                 })]
             })), M("text", {
                 x: pe / 2,
                 y: I,
                 class: "qs-scatterChart-x-axisTitle",
                 children: [r.xAxis.label, " (logarithmic)"]
             }), M("text", {
-                x: L - G,
+                x: L - O,
                 y: ue / 2,
                 class: "qs-scatterChart-y-axisTitle",
                 children: [r.yAxis.label, " (logarithmic)"]
             }), M("text", {
                 class: "qs-scatterChart-watermark",
-                x: L - G,
+                x: L - O,
                 y: -te + I,
                 children: "Created with Azure Quantum Resource Estimator"
             }), M("g", {
                 children: r.data.map((ae, ee) => {
-                    let $ = ae.items.map(Te => ({
+                    let G = ae.items.map(Te => ({
                             x: g(Te.x),
                             y: y(Te.y)
                         })),
-                        fe = $.map(Te => `${Te.x},${Te.y}`).join(" ");
+                        fe = G.map(Te => `${Te.x},${Te.y}`).join(" ");
                     return M(Ge, {
                         children: [ae.items.map((Te, Ae) => M("circle", {
                             "data-index": JSON.stringify([ee, Ae]),
                             "data-label": Te.label,
                             className: "qs-scatterChart-point qs-scatterChart-hover",
-                            cx: $[Ae].x,
-                            cy: $[Ae].y,
+                            cx: G[Ae].x,
+                            cy: G[Ae].y,
                             stroke: ae.color
                         }, Ae)), M("polyline", {
                             points: fe,
                             stroke: ae.color,
                             fill: "none"
                         })]
                     })
@@ -17793,50 +17798,50 @@
             ref: e
         }), M("div", {
             class: "qs-scatterChart-tooltip"
         })]
     })
 }
 
-function Ra(r) {
+function La(r) {
     let e = [],
         i = 1.4142135623730951,
         a = .618033988749895,
         l = 2.718281828459045;
     for (let c = 0; c < r; c++) {
         let d = c * a % 1,
-            m = (1 - c * i % 1) * .5 + .5,
+            f = (1 - c * i % 1) * .5 + .5,
             g = c * l % 1 * .3 + .35,
-            y = Sh(d, m, g),
-            _ = Ch(y[0], y[1], y[2]);
+            y = Ch(d, f, g),
+            _ = Th(y[0], y[1], y[2]);
         e.push(_)
     }
     return e
 }
 
-function Sh(r, e, i) {
+function Ch(r, e, i) {
     let a, l, c;
     if (e === 0) a = l = c = i;
     else {
-        let d = (y, _, k) => (k < 0 && (k += 1), k > 1 && (k -= 1), k < .16666666666666666 ? y + (_ - y) * 6 * k : k < .5 ? _ : k < .6666666666666666 ? y + (_ - y) * (.6666666666666666 - k) * 6 : y),
-            m = i < .5 ? i * (1 + e) : i + e - i * e,
-            g = 2 * i - m;
-        a = d(g, m, r + 1 / 3), l = d(g, m, r), c = d(g, m, r - 1 / 3)
+        let d = (y, _, w) => (w < 0 && (w += 1), w > 1 && (w -= 1), w < .16666666666666666 ? y + (_ - y) * 6 * w : w < .5 ? _ : w < .6666666666666666 ? y + (_ - y) * (.6666666666666666 - w) * 6 : y),
+            f = i < .5 ? i * (1 + e) : i + e - i * e,
+            g = 2 * i - f;
+        a = d(g, f, r + 1 / 3), l = d(g, f, r), c = d(g, f, r - 1 / 3)
     }
     return [Math.round(a * 255), Math.round(l * 255), Math.round(c * 255)]
 }
 
-function Ch(r, e, i) {
+function Th(r, e, i) {
     return `#${(1<<24|r<<16|e<<8|i).toString(16).slice(1).toUpperCase()}`
 }
 
-function Fa(r) {
-    let [e, i] = Ke(r.initialColumns), [a, l] = Ke(null), [c, d] = Ke(!1), [m, g] = Ke(""), y = St(""), _ = St(null);
+function Pa(r) {
+    let [e, i] = Xe(r.initialColumns), [a, l] = Xe(null), [c, d] = Xe(!1), [f, g] = Xe(""), y = St(""), _ = St(null);
 
-    function k(U) {
+    function w(U) {
         if (!(U.target instanceof HTMLElement)) return;
         let X = U.target.closest("th")?.dataset.colid;
         y.current = X, U.dataTransfer.dropEffect = "move"
     }
 
     function T(U) {
         if (!(U.target instanceof HTMLElement)) return;
@@ -17856,15 +17861,15 @@
 
     function R(U) {
         if (!(U.target instanceof HTMLElement)) return;
         let X = U.target.closest("th")?.dataset.colid;
         X && (U.target.closest("table").querySelectorAll(`[data-colid="${X}"]`).forEach(he => he.classList.remove("qs-resultsTable-dragEnter")), U.preventDefault())
     }
 
-    function G(U) {
+    function O(U) {
         if (!(U.target instanceof HTMLElement)) return;
         let X = U.target.closest("th")?.dataset.colid;
         X && y.current && (I(parseInt(y.current), parseInt(X)), U.preventDefault())
     }
 
     function P(U) {
         U.target.closest("table").querySelectorAll("th, td").forEach(X => X.classList.remove("qs-resultsTable-dragEnter")), y.current = ""
@@ -17892,31 +17897,31 @@
 
     function re(U) {
         if (!a) return U;
         let X = a.columnId,
             he = a.ascending,
             oe = [...U];
         return oe.sort((ae, ee) => {
-            let $ = ae.cells[X],
+            let G = ae.cells[X],
                 fe = ee.cells[X];
-            return typeof $ == "string" && typeof fe == "string" ? he ? $.localeCompare(fe) : fe.localeCompare($) : typeof $ == "number" && typeof fe == "number" ? he ? $ - fe : fe - $ : typeof $ == "object" && typeof fe == "object" ? he ? $.sortBy - fe.sortBy : fe.sortBy - $.sortBy : 0
+            return typeof G == "string" && typeof fe == "string" ? he ? G.localeCompare(fe) : fe.localeCompare(G) : typeof G == "number" && typeof fe == "number" ? he ? G - fe : fe - G : typeof G == "object" && typeof fe == "object" ? he ? G.sortBy - fe.sortBy : fe.sortBy - G.sortBy : 0
         }), oe
     }
 
     function te(U) {
         return typeof U == "object" ? U.value : typeof U == "number" ? U.toLocaleString() : U || ""
     }
 
     function j(U) {
         let X = r.selectedRow === U ? "" : U;
         A(X)
     }
 
     function ne(U, X) {
-        U.stopPropagation(), g(m === X ? "" : X)
+        U.stopPropagation(), g(f === X ? "" : X)
     }
 
     function pe(U) {
         U.stopPropagation(), g(""), d(!c)
     }
 
     function ue() {
@@ -17947,15 +17952,15 @@
                 break;
             case "ArrowUp":
                 he > 0 && (U.preventDefault(), r.onRowSelected(X[he - 1]));
                 break;
             default:
         }
     }
-    return cr(() => {
+    return Ut(() => {
         c && _.current && _.current.focus()
     }), M("table", {
         class: "qs-resultsTable-sortedTable",
         tabIndex: 0,
         onKeyDown: De,
         children: [M("thead", {
             children: M("tr", {
@@ -18006,20 +18011,20 @@
                     let X = a?.columnId === U;
                     return M("th", {
                         onClick: Y,
                         "data-colid": U.toString(),
                         children: [M("span", {
                             class: X ? "qs-resultsTable-sortHeaderCell" : "qs-resultsTable-headerCell",
                             draggable: !0,
-                            onDragStart: k,
+                            onDragStart: w,
                             onDragEnter: T,
                             onDragOver: L,
                             onDragLeave: R,
                             onDragEnd: P,
-                            onDrop: G,
+                            onDrop: O,
                             children: r.columnNames[U]
                         }), X ? M("svg", {
                             width: "16",
                             height: "16",
                             style: `transform: rotate(${a.ascending?"0":"180"}deg)`,
                             children: M("polygon", {
                                 fill: "gray",
@@ -18046,15 +18051,15 @@
                                 style: "position: relative;",
                                 children: M("path", {
                                     "stroke-width": "1.5",
                                     stroke: U.color,
                                     "stroke-linecap": "round",
                                     d: "M4,5 h8 M4,8 h8 M4,11 h8"
                                 })
-                            }), m === X ? M("div", {
+                            }), f === X ? M("div", {
                                 class: "qs-resultsTable-showColumnMenu",
                                 style: "top: 16px; left: 0px;",
                                 children: M("div", {
                                     class: "qs-resultsTable-menuItem",
                                     onClick: he => Ce(he, X),
                                     children: "Delete"
                                 })
@@ -18065,157 +18070,171 @@
                         children: te(U.cells[he])
                     }))]
                 })
             })
         })]
     })
 }
-var Th = ["Run name", "Estimate type", "Qubit type", "QEC scheme", "Error budget", "Logical qubits", "Logical depth", "Code distance", "T states", "T factories", "T factory fraction", "Runtime", "rQOPS", "Physical qubits"],
-    Ah = [0, 10, 13, 11, 12],
-    qh = {
+var Ah = ["Run name", "Estimate type", "Qubit type", "QEC scheme", "Error budget", "Logical qubits", "Logical depth", "Code distance", "T states", "T factories", "T factory fraction", "Runtime", "rQOPS", "Physical qubits"],
+    qh = [0, 10, 13, 11, 12],
+    Mh = {
         isTime: !0,
         label: "Runtime"
     },
-    Mh = {
+    Eh = {
         isTime: !1,
         label: "Physical qubits"
     };
 
-function Eh(r, e) {
+function Dh(r, e) {
     let i = jt(r, 0),
         a = r.frontierEntries == null ? "Single" : "Frontier (" + r.frontierEntries.length + "  items)";
     return {
         cells: [i.jobParams.runName, a, i.jobParams.qubitParams.name, i.jobParams.qecScheme.name, i.jobParams.errorBudget, i.physicalCounts.breakdown.algorithmicLogicalQubits, i.physicalCounts.breakdown.algorithmicLogicalDepth, i.logicalQubit.codeDistance, i.physicalCounts.breakdown.numTstates, i.physicalCounts.breakdown.numTfactories, i.physicalCountsFormatted.physicalQubitsForTfactoriesPercentage, {
             value: i.physicalCountsFormatted.runtime,
             sortBy: i.physicalCounts.runtime
         }, i.physicalCounts.rqops, i.physicalCounts.physicalQubits],
         color: e
     }
 }
 
-function Dh(r) {
+function zh(r) {
     return {
         x: r.physicalCounts.runtime,
         y: r.physicalCounts.physicalQubits,
         label: r.physicalCountsFormatted.runtime + ", physical qubits: " + r.physicalCountsFormatted.physicalQubits + ", code distance: " + r.logicalQubit.codeDistance
     }
 }
 
-function zh(r, e) {
+function Rh(r, e) {
     return r.frontierEntries == null || r.frontierEntries.length === 0 ? {
         color: e,
         items: [{
             x: r.physicalCounts.runtime,
             y: r.physicalCounts.physicalQubits,
             label: r.physicalCountsFormatted.runtime + ", physical qubits: " + r.physicalCountsFormatted.physicalQubits + ", code distance: " + r.logicalQubit.codeDistance
         }]
     } : {
         color: e,
-        items: r.frontierEntries.map(Dh)
+        items: r.frontierEntries.map(zh)
     }
 }
 
-function Rh(r) {
+function Fh(r) {
     if (r.length === 1) return [r[0].jobParams.sharedRunName ?? r[0].jobParams.qubitParams.name ?? r[0].jobParams.qecScheme.name ?? "estimate"];
     let e = [];
     r.forEach(() => {
         e.push([])
-    }), g0(e, r, a => a.jobParams.sharedRunName), g0(e, r, a => a.jobParams.qubitParams.name), g0(e, r, a => a.jobParams.qecScheme.name), g0(e, r, a => String(a.jobParams.errorBudget));
+    }), b0(e, r, a => a.jobParams.sharedRunName), b0(e, r, a => a.jobParams.qubitParams.name), b0(e, r, a => a.jobParams.qecScheme.name), b0(e, r, a => String(a.jobParams.errorBudget));
     let i = e.map(a => a.join(", "));
     return new Set(i).size != i.length ? i.map((a, l) => a + " (" + l + ")") : i
 }
 
-function g0(r, e, i) {
+function b0(r, e, i) {
     let a = e.map(i);
     new Set(a).size > 1 && a.forEach((c, d) => {
         r[d].push(c)
     })
 }
 
 function Er(r) {
-    let [e, i] = Ke(null), [a, l] = Ke(), c = r.runNames != null && r.runNames.length > 0 && r.runNames.length != r.estimatesData.length ? "Warning: The number of runNames does not match the number of estimates. Ignoring provided runNames." : "", d = r.runNames != null && r.runNames.length == r.estimatesData.length ? r.runNames : Rh(r.estimatesData);
+    let [e, i] = Xe(null), [a, l] = Xe(), c = r.runNames != null && r.runNames.length > 0 && r.runNames.length != r.estimatesData.length ? "Warning: The number of runNames does not match the number of estimates. Ignoring provided runNames." : "", d = r.runNames != null && r.runNames.length == r.estimatesData.length ? r.runNames : Fh(r.estimatesData);
     r.estimatesData.forEach((A, L) => {
         A.jobParams.runName = d[L]
     });
 
-    function m(A, L) {
+    function f(A, L) {
         if (A < 0) {
             g("");
             return
         }
         let R = r.estimatesData[A];
         r.setEstimate(jt(R, L));
-        let G = r.estimatesData[A].jobParams.runName;
-        i(G), l([A, L])
+        let O = r.estimatesData[A].jobParams.runName;
+        i(O), l([A, L])
     }
 
     function g(A) {
         if (i(A), !A) r.setEstimate(null), l(void 0);
         else {
             let L = r.estimatesData.findIndex(R => R.jobParams.runName === A);
             if (L == -1) r.setEstimate(null), l(void 0);
             else {
                 let R = r.estimatesData[L];
                 l([L, 0]), r.setEstimate(jt(R, 0))
             }
         }
     }
     let y = r.colors != null && r.colors.length > 0 && r.colors.length != r.estimatesData.length ? "Warning: The number of colors does not match the number of estimates. Ignoring provided colors." : "",
-        _ = r.colors != null && r.colors.length == r.estimatesData.length ? r.colors : Ra(r.estimatesData.length);
+        _ = r.colors != null && r.colors.length == r.estimatesData.length ? r.colors : La(r.estimatesData.length);
 
-    function k() {
-        return M(Fa, {
-            columnNames: Th,
-            rows: r.estimatesData.map((A, L) => Eh(A, _[L])),
-            initialColumns: Ah,
+    function w() {
+        return M(Pa, {
+            columnNames: Ah,
+            rows: r.estimatesData.map((A, L) => Dh(A, _[L])),
+            initialColumns: qh,
             selectedRow: e,
             onRowSelected: g,
             onRowDeleted: r.onRowDeleted
         })
     }
 
     function T() {
-        return M(Pn, {
-            xAxis: qh,
-            yAxis: Mh,
-            data: r.estimatesData.map((A, L) => zh(A, _[L])),
-            onPointSelected: m,
+        return M(In, {
+            xAxis: Mh,
+            yAxis: Eh,
+            data: r.estimatesData.map((A, L) => Rh(A, _[L])),
+            onPointSelected: f,
             selectedPoint: a
         })
     }
     return M("div", {
         className: "qs-estimatesOverview",
         children: [c != "" && M("div", {
             class: "qs-estimatesOverview-error",
             children: c
         }), y != "" && M("div", {
             class: "qs-estimatesOverview-error",
             children: y
         }), r.isSimplifiedView ? M(Ge, {
-            children: [k(), T()]
+            children: [w(), T()]
         }) : M(Ge, {
             children: [M("details", {
                 open: !0,
                 children: [M("summary", {
                     style: "font-size: 1.5em; font-weight: bold; margin: 24px 8px;",
                     children: "Results"
-                }), k()]
+                }), w()]
             }), M("details", {
                 open: !0,
                 children: [M("summary", {
                     style: "font-size: 1.5em; font-weight: bold; margin: 24px 8px;",
                     children: "Space-time diagram"
                 }), T()]
             })]
         })]
     })
 }
 
-function In(r) {
-    let [e, i] = Ke(null);
+function On(r) {
+    return M("svg", {
+        width: "40",
+        height: "40",
+        viewBox: "0 0 16 16",
+        xmlns: "http://www.w3.org/2000/svg",
+        class: "codicon-modifier-spin",
+        style: r.style,
+        children: M("path", {
+            d: "M2.006 8.267L.78 9.5 0 8.73l2.09-2.07.76.01 2.09 2.12-.76.76-1.167-1.18a5 5 0 0 0 9.4 1.983l.813.597a6 6 0 0 1-11.22-2.683zm10.99-.466L11.76 6.55l-.76.76 2.09 2.11.76.01 2.09-2.07-.75-.76-1.194 1.18a6 6 0 0 0-11.11-2.92l.81.594a5 5 0 0 1 9.3 2.346z"
+        })
+    })
+}
+
+function Hn(r) {
+    let [e, i] = Xe(null);
     return M(Ge, {
         children: [M("div", {
             style: "display:flex; height:64px; align-items: center; position: relative",
             children: [M("svg", {
                 width: "48",
                 height: "48",
                 viewBox: "96 96 828 828",
@@ -18266,24 +18285,16 @@
                         d: "M 665 845 L 816 758"
                     }), M("path", {
                         d: "M 433 801 L 820 577"
                     }), M("path", {
                         d: "M 820 489 L 360 755"
                     })]
                 })
-            }), r.calculating ? M("svg", {
-                width: "40",
-                height: "40",
-                viewBox: "0 0 16 16",
-                xmlns: "http://www.w3.org/2000/svg",
-                class: "codicon-modifier-spin",
-                style: "position: absolute; top: 11px; left: 4px;",
-                children: M("path", {
-                    d: "M2.006 8.267L.78 9.5 0 8.73l2.09-2.07.76.01 2.09 2.12-.76.76-1.167-1.18a5 5 0 0 0 9.4 1.983l.813.597a6 6 0 0 1-11.22-2.683zm10.99-.466L11.76 6.55l-.76.76 2.09 2.11.76.01 2.09-2.07-.75-.76-1.194 1.18a6 6 0 0 0-11.11-2.92l.81.594a5 5 0 0 1 9.3 2.346z"
-                })
+            }), r.calculating ? M(On, {
+                style: "position: absolute; top: 11px; left: 4px;"
             }) : null, M("h1", {
                 children: "Azure Quantum Resource Estimator"
             })]
         }), M(Er, {
             estimatesData: r.estimatesData,
             isSimplifiedView: !1,
             onRowDeleted: r.onRowDeleted,
@@ -18308,225 +18319,294 @@
                     mdRenderer: r.renderer,
                     estimatesData: e
                 })]
             })]
         }) : null]
     })
 }
-var hs = qn(ls(), 1);
-var cs = 1e4,
-    us = 1e3;
+var ms = Mn(ds(), 1);
+var ei = 1e4,
+    ti = 1e3;
+
+function ri(r) {
+    let e = r.circuit,
+        i = e.qubits.length === 0 || e.operations.length > ei || e.qubits.length > ti;
+    return M("div", {
+        children: i ? M(wd, {
+            qubits: r.circuit.qubits.length,
+            operations: r.circuit.operations.length
+        }) : M(vd, {
+            circuit: r.circuit
+        })
+    })
+}
 
-function Jn(r) {
+function vd(r) {
     let e = St(null),
-        i = r.circuit.qubits.length === 0 ? M("div", {
-            children: M("p", {
-                children: "No circuit to display. No qubits have been allocated."
-            })
-        }) : r.circuit.operations.length > cs ? M("div", {
-            children: M("p", {
-                children: ["This circuit has too many gates to display. It has", " ", r.circuit.operations.length, " gates, but the maximum supported is", " ", cs, "."]
-            })
-        }) : r.circuit.qubits.length > us ? M("div", {
-            children: M("p", {
-                children: ["This circuit has too many qubits to display. It has", " ", r.circuit.qubits.length, " qubits, but the maximum supported is", " ", us, "."]
-            })
-        }) : void 0;
-    return cr(() => {
-        if (i !== void 0) {
-            e.current.innerHTML = "";
-            return
-        }
-        hs.draw(r.circuit, e.current), e.current?.querySelectorAll("style")?.forEach(l => l.remove())
-    }, [r.circuit]), M("div", {
+        [i, a] = Xe(100),
+        [l, c] = Xe(!0);
+    return Ut(() => {
+        c(!0);
+        let y = e.current;
+        y.innerHTML = ""
+    }, [r.circuit]), Ut(() => {
+        if (l) {
+            let y = e.current,
+                _ = f(r.circuit, y),
+                w = g(y, _);
+            a(w), d(), c(!1)
+        }
+    }, [l]), Ut(() => {
+        d()
+    }, [i]), M("div", {
         children: [M("div", {
-            class: "qs-circuit-error",
-            children: i
+            children: l ? null : M(kd, {
+                zoom: i,
+                onChange: a
+            })
+        }), M("div", {
+            children: l ? `Rendering diagram with ${r.circuit.operations.length} gates...` : ""
         }), M("div", {
             class: "qs-circuit",
             ref: e
         })]
+    });
+
+    function d() {
+        let y = e.current?.querySelector(".qviz");
+        if (y) {
+            let _ = y.getAttribute("width");
+            y.setAttribute("style", `max-width: ${_}; width: ${parseInt(_)*(i||100)/100}; height: auto`)
+        }
+    }
+
+    function f(y, _) {
+        return ms.draw(y, _), _.querySelectorAll("style")?.forEach(T => T.remove()), _.getElementsByClassName("qviz")[0]
+    }
+
+    function g(y, _) {
+        let w = y.clientWidth,
+            T = parseInt(_.getAttribute("width")),
+            A = _.getAttribute("height");
+        return _.setAttribute("viewBox", `0 0 ${T} ${A}`), Math.min(Math.ceil(w / T * 100), 100)
+    }
+}
+
+function wd(r) {
+    let e = r.qubits === 0 ? M("div", {
+        children: M("p", {
+            children: "No circuit to display. No qubits have been allocated."
+        })
+    }) : r.operations > ei ? M("div", {
+        children: M("p", {
+            children: ["This circuit has too many gates to display. It has ", r.operations, " ", "gates, but the maximum supported is ", ei, "."]
+        })
+    }) : r.qubits > ti ? M("div", {
+        children: M("p", {
+            children: ["This circuit has too many qubits to display. It has ", r.qubits, " ", "qubits, but the maximum supported is ", ti, "."]
+        })
+    }) : void 0;
+    return M("div", {
+        class: "qs-circuit-error",
+        children: e
+    })
+}
+
+function kd(r) {
+    return M("p", {
+        children: [M("label", {
+            htmlFor: "qs-circuit-zoom",
+            children: "Zoom "
+        }), M("input", {
+            id: "qs-circuit-zoom",
+            type: "number",
+            min: "10",
+            max: "100",
+            step: "10",
+            value: r.zoom,
+            onInput: e => r.onChange(parseInt(e.target.value) || 0)
+        }), "%"]
     })
 }
-var Tu = qn(gu()),
-    Au = qn(Cu());
-var qu = (0, Tu.default)();
-qu.use(Au.default);
+var Au = Mn(yu()),
+    qu = Mn(Tu());
+var Mu = (0, Au.default)();
+Mu.use(qu.default);
 
-function Mu(r) {
-    return qu.render(r.replace(/\\\\/g, "\\"))
+function Eu(r) {
+    return Mu.render(r.replace(/\\\\/g, "\\"))
 }
 
-function W2({
+function n5({
     model: r,
     el: e
 }) {
     let i = r.get("comp");
     switch (i) {
         case "SpaceChart":
-            Ip({
+            jp({
                 model: r,
                 el: e
             });
             break;
         case "EstimatesOverview":
-            Op({
+            Up({
                 model: r,
                 el: e
             });
             break;
         case "EstimateDetails":
-            Pp({
+            Vp({
                 model: r,
                 el: e
             });
             break;
         case "Histogram":
-            $p({
+            Yp({
                 model: r,
                 el: e
             });
             break;
         case "EstimatesPanel":
-            Hp({
+            Wp({
                 model: r,
                 el: e
             });
             break;
         case "Circuit":
-            Gp({
+            Zp({
                 model: r,
                 el: e
             });
             break;
         default:
             throw new Error(`Unknown component type ${i}`)
     }
 }
 
-function Pp({
+function Vp({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("estimates"),
             l = r.get("index"),
             c = jt(a, l);
-        tr(M(qr, {
+        rr(M(qr, {
             estimatesData: c,
-            mdRenderer: Mu
+            mdRenderer: Eu
         }), e)
     };
     i(), r.on("change:estimates", i), r.on("change:index", i)
 }
 
-function Ip({
+function jp({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("estimates"),
             l = r.get("index"),
             c = jt(a, l);
-        tr(M(Mr, {
+        rr(M(Mr, {
             estimatesData: c
         }), e)
     };
     i(), r.on("change:estimates", i), r.on("change:index", i)
 }
 
-function Op({
+function Up({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("estimates"),
             l = r.get("colors"),
             c = r.get("runNames"),
             d = [];
         if (a[0] == null) d.push(a);
         else
             for (let g of Object.values(a)) d.push(g);
-        let m = Eu(d, g => {
+        let f = Du(d, g => {
             d = g, r.set("estimates", d)
         });
-        tr(M(Er, {
+        rr(M(Er, {
             estimatesData: d,
             runNames: c,
             colors: l,
             isSimplifiedView: !0,
-            onRowDeleted: m,
+            onRowDeleted: f,
             setEstimate: () => {}
         }), e)
     };
     i(), r.on("change:estimates", i), r.on("change:colors", i), r.on("change:runNames", i)
 }
 
-function Hp({
+function Wp({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("estimates"),
             l = r.get("colors"),
             c = r.get("runNames"),
             d = [];
         if (a[0] == null) d.push(a);
         else
             for (let g of Object.values(a)) d.push(g);
-        let m = Eu(d, g => {
+        let f = Du(d, g => {
             d = g, r.set("estimates", d)
         });
-        tr(M(In, {
+        rr(M(Hn, {
             estimatesData: d,
             runNames: c,
             colors: l,
-            renderer: Mu,
+            renderer: Eu,
             calculating: !1,
-            onRowDeleted: m
+            onRowDeleted: f
         }), e)
     };
     i(), r.on("change:estimates", i), r.on("change:colors", i), r.on("change:runNames", i)
 }
 
-function Eu(r, e) {
+function Du(r, e) {
     return i => {
         let a = JSON.parse(JSON.stringify(r)),
             l = a.findIndex(c => c.jobParams.runName === i);
         l >= 0 && a.splice(l, 1), e(a)
     }
 }
 
-function $p({
+function Yp({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("buckets"),
             l = new Map(Object.entries(a)),
             c = r.get("shot_count");
-        tr(M(Ln, {
+        rr(M(Pn, {
             data: l,
             shotCount: c,
             filter: "",
             onFilter: () => {},
             shotsHeader: !0
         }), e)
     };
     i(), r.on("change:buckets", i), r.on("change:shot_count", i)
 }
 
-function Gp({
+function Zp({
     model: r,
     el: e
 }) {
     let i = () => {
         let a = r.get("circuit_json");
-        tr(M(Jn, {
+        rr(M(ri, {
             circuit: JSON.parse(a)
         }), e)
     };
     i(), r.on("change:circuit_json", i)
 }
 export {
-    Mu as mdRenderer, W2 as render
+    Eu as mdRenderer, n5 as render
 };
```

