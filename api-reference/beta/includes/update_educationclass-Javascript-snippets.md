---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8f289de401a0c867feb2f90ee0cd796f724714b9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationClass = {
  description: "History - World History 1",
  displayName: "World History Level 1",
};

let res = await client.api('/education/classes/11014')
    .version('beta')
    .update({educationClass : educationClass});

```