---
id: pvlzpktu
title: A doc
file_version: 1.1.3
app_version: 1.11.0
---


<!-- NOTE-swimm-snippet: the lines below link your snippet to Swimm -->
### 📄 js/dist/util/component-functions.js
```javascript
2        * Bootstrap component-functions.js v5.3.0-alpha3 (https://getbootstrap.com/)
3        * Copyright 2011-2023 The Bootstrap Authors (https://github.com/twbs/bootstrap/graphs/contributors)
4        * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE)
5        */
6      (function (global, factory) {
7        typeof exports === 'object' && typeof module !== 'undefined' ? factory(exports, require('../dom/event-handler.js'), require('../dom/selector-engine.js'), require('./index.js')) :
8        typeof define === 'function' && define.amd ? define(['exports', '../dom/event-handler', '../dom/selector-engine', './index'], factory) :
9        (global = typeof globalThis !== 'undefined' ? globalThis : global || self, factory(global.ComponentFunctions = {}, global.EventHandler, global.SelectorEngine, global.Index));
10     })(this, (function (exports, EventHandler, SelectorEngine, index_js) { 'use strict';
11     
12       /**
13        * --------------------------------------------------------------------------
14        * Bootstrap util/component-functions.js
15        * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE)
16        * --------------------------------------------------------------------------
17        */
18       const enableDismissTrigger = (component, method = 'hide') => {
19         const clickEvent = `click.dismiss${component.EVENT_KEY}`;
20         const name = component.NAME;
21         EventHandler.on(document, clickEvent, `[data-bs-dismiss="${name}"]`, function (event) {
22           if (['A', 'AREA'].includes(this.tagName)) {
23             event.preventDefault();
24           }
25           if (index_js.isDisabled(this)) {
26             return;
```

<br/>

This file was generated by Swimm. [Click here to view it in the app](https://swimm-web-app.web.app/repos/Z2l0aHViJTNBJTNBYm9vdHN0cmFwJTNBJTNBSWRpdFllZ2VyU3dpbW0=/docs/pvlzpktu).
