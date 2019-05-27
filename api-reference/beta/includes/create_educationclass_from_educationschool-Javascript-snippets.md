---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cef07a40c27b4fd3ccccd16fe1daffc1fe9dfe5e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480997"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
 @odata.id:"https://graph.microsoft.com/beta/education/classes/11006"
};

let res = await client.api('/education/schools/10002/classes/$ref')
    .version('beta')
    .post({educationClass : educationClass});

```