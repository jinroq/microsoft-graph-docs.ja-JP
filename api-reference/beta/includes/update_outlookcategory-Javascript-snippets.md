---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ddbac2686d52d5249e94cfb8ec5f7363098382d5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
  color:"preset15"
};

let res = await client.api('/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac')
    .version('beta')
    .update({outlookCategory : outlookCategory});

```