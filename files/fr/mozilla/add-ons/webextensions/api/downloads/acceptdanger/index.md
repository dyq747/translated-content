---
title: downloads.acceptDanger()
slug: Mozilla/Add-ons/WebExtensions/API/downloads/acceptDanger
---

{{AddonSidebar}}

La fonction **`acceptDanger()`** de l'API {{WebExtAPIRef("downloads")}} invite l'utilisateur à accepter ou à annuler un téléchargement potentiellement dangereux.

Cette fonction ne peut pas être appelée à partir de scripts d'arrière-plan, uniquement dans les scripts qui s'exécutent dans une fenêtre visible (par exemple un navigateur ou une fenêtre d'action de page).

C'est une fonction asynchrone qui renvoie une [`Promise`](/fr/docs/Web/JavaScript/Reference/Global_Objects/Promise).

## Syntaxe

```js
var prompting = browser.downloads.acceptDanger(
  downloadId, // integer
);
```

### Parameters

- `downloadId`
  - : Un `integer` représentant l'`id` de {{WebExtAPIRef("downloads.DownloadItem", "DownloadItem")}} en question.

### Valeur retournée

Une [`Promise`](/fr/docs/Web/JavaScript/Reference/Global_Objects/Promise). Lorsque la boîte de dialogue se ferme, la promesse sera remplie sans arguments.

## Compatibilité des navigateurs

{{Compat}}

{{WebExtExamples}}

> [!NOTE]
>
> Cette API est basée sur l'API Chromium [`chrome.downloads`](https://developer.chrome.com/docs/extensions/reference/api/downloads).
>
> Les données de compatibilité relatives à Microsoft Edge sont fournies par Microsoft Corporation et incluses ici sous la licence Creative Commons Attribution 3.0 pour les États-Unis.

<!--
// Copyright 2015 The Chromium Authors. All rights reserved.
//
// Redistribution and use in source and binary forms, with or without
// modification, are permitted provided that the following conditions are
// met:
//
//    * Redistributions of source code must retain the above copyright
// notice, this list of conditions and the following disclaimer.
//    * Redistributions in binary form must reproduce the above
// copyright notice, this list of conditions and the following disclaimer
// in the documentation and/or other materials provided with the
// distribution.
//    * Neither the name of Google Inc. nor the names of its
// contributors may be used to endorse or promote products derived from
// this software without specific prior written permission.
//
// THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
// "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
// LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
// A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
// OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
// SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
// LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
// DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
// THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
// (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
// OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-->
